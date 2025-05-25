# StreamTodo

StreamTodo is a lightweight, interactive Todo application built with Streamlit’s Python-first web framework and SQLAlchemy’s Core API for persistence. It lets you create, read, update, and delete tasks—all in a clean, easy-to-use interface with SQL database backing.

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
   cd streamtodo
