Overview
The Streamlit Todo App is a lightweight task manager built with Streamlit’s Python‐first UI framework and SQLAlchemy’s Core API for persistence. It defines a Todo dataclass to represent each task, renders interactive forms and buttons for CRUD operations, caches the table metadata for efficiency, and stores session state for a smooth user experience 
PyPI
SQLAlchemy
 
Python documentation
Streamlit Docs
.

Features
Create / Read / Update / Delete Todos via intuitive Streamlit forms and buttons 
Streamlit Docs
.

Batch form submissions with st.form and st.form_submit_button to avoid unnecessary reruns 
Streamlit Docs
.

Session state management to remember task lists and editing flags across reruns 
Streamlit Docs
.

Global resource caching of the SQLAlchemy MetaData and Table objects using @st.cache_resource for performance and thread safety 
Streamlit Docs
.

Database connections via st.connection(...), automatically cached under the hood 
Streamlit Docs
.

Installation
Clone the repo:

bash
Copy
Edit
git clone https://github.com/yourusername/streamlit-todo-app.git
cd streamlit-todo-app
Create and activate a virtual environment (Python 3.7+ recommended):

bash
Copy
Edit
python3 -m venv venv
source venv/bin/activate   # on Unix/macOS
.\venv\Scripts\activate    # on Windows
Install dependencies:

bash
Copy
Edit
pip install streamlit sqlalchemy
Streamlit for the UI 
PyPI

SQLAlchemy for database interaction 
SQLAlchemy

Usage
Run the app locally with:

bash
Copy
Edit
streamlit run app.py
The browser will open to http://localhost:8501 by default.

Create the database table via the “Create table” button in the sidebar.

Add, edit, delete, and mark todos directly in the web interface.

Configuration
– The script calls st.set_page_config(...) at the top to set the page title, icon, and initial sidebar state; this must be the first Streamlit call in your app 
Streamlit Docs
.
– You can tweak caching parameters (e.g. TTL) on the @st.cache_resource decorator to control resource lifetime.

Project Structure
bash
Copy
Edit
.
├── app.py               # Main Streamlit application
├── requirements.txt     # Pinned minimal dependencies
└── README.md            # This file
