# TodoStream

A fluid, Python-powered task manager built with Streamlit and SQLAlchemy.
TodoStream is a lightweight, interactive Todo application built with Streamlit’s Python-first web framework and SQLAlchemy’s Core API for persistence. It lets you create, read, update, and delete tasks—all in a clean, easy-to-use interface with SQL database backing.

---

## Table of Contents

- [Features](#features)  
- [Demo](#demo)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Configuration](#configuration)  
- [Project Structure](#project-structure)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Features

- **CRUD Operations**  
  Create, read, update, and delete tasks with intuitive Streamlit forms and buttons.  
- **Session State Management**  
  Remember your current list of todos and editing state across interactions.  
- **Cached Resources**  
  Define your SQLAlchemy table schema once with `@st.cache_resource` for speed and thread safety.  
- **Database Connections**  
  Connect via `st.connection("todo_db")`, supporting SQLite (default) or other SQL engines.  
- **Clean, Modern UI**  
  Leverage Streamlit’s layout primitives—forms, columns, containers—for a polished look.  

---

## Demo

![StreamTodo Demo](https://user-images.githubusercontent.com/yourusername/streamtodo-demo.gif)

---

## Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/yourusername/streamtodo.git
   cd streamtodo```
Create and activate a virtual environment

bash
Copy
Edit
python3 -m venv venv
# On macOS/Linux:
source venv/bin/activate
# On Windows:
.\venv\Scripts\activate
2. **Install dependencies**

```pip install streamlit sqlalchemy```
## Usage
**Run the app locally:**

```streamlit run app.py```
Open your browser to http://localhost:8501.

In the Admin sidebar, click Create Table to initialize the database.

Add, edit, delete, and mark todos directly from the web interface.

3. **Configuration**

Page Settings
Controlled by st.set_page_config at the top of app.py.

Cache TTL
Adjust the Time-To-Live on the @st.cache_resource decorator to control metadata caching.

4. **Project Structure**

  ```streamtodo/
  ├── app.py              # Main Streamlit application
  ├── requirements.txt    # Minimal pinned dependencies
  └── README.md```           # Project documentation
