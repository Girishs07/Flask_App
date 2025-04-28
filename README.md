


# Flask App

This is a simple Flask application for managing a to-do list. The application is connected to a MySQL database, allowing users to add, update, and delete tasks.

## Features
- Add tasks
- Update tasks
- Delete tasks
- View tasks in a list format

## Tools & Technologies Used
- **Flask**: A lightweight Python web framework used for building the web application.
- **MySQL**: A relational database used to store the to-do list tasks.
- **Jinja2**: Template engine used for rendering HTML.
- **Bootstrap**: For front-end styling (optional, if used in the project).

## Running the Flask App

Follow these steps to run the Flask app on your local machine:

### 1. Clone the Repository

First, clone the repository to your local machine:
```bash
git clone https://github.com/Girishs07/Flask_App.git
```

### 2. Navigate to the Project Directory

Change into the project directory:
```bash
cd Flask_App
```

### 3. Set Up a Virtual Environment

It's a good practice to use a virtual environment to manage dependencies. Create a virtual environment with the following command:
```bash
python -m venv venv
```

### 4. Activate the Virtual Environment

- **On Windows**:
  ```bash
  venv\Scripts\activate
  ```
- **On macOS/Linux**:
  ```bash
  source venv/bin/activate
  ```

### 5. Install Dependencies

With the virtual environment activated, install the required Python dependencies:
```bash
pip install -r requirements.txt
```

### 6. Set Up the MySQL Database

Make sure MySQL is installed and running on your machine.

1. Create a new MySQL database:
   ```sql
   CREATE DATABASE flask_todolist;
   ```

2. Update the database connection details in your Flask app (typically in `app.py` or `__init__.py`). For example:
   ```python
   import mysql.connector

   db = mysql.connector.connect(
       host="localhost",
       user="your_username",
       password="your_password",
       database="flask_todolist"
   )
   ```

### 7. Run the Flask App

You can now run the Flask app using the following command:
```bash
python app.py
```

This will start the app on `http://127.0.0.1:5000/` by default.

Alternatively, you can also run it using the Flask CLI:
```bash
flask run
```

### 8. Access the Application

Open your web browser and visit:
[http://127.0.0.1:5000/](http://127.0.0.1:5000/) to start using the To-Do List app.

### 9. Troubleshooting

- If you face issues with the database connection, ensure that your MySQL service is running and the credentials are correct.
- If you encounter any missing dependencies, try running:
  ```bash
  pip install <missing_package>
  ```

### 10. Stopping the Flask App

To stop the Flask app, you can press `Ctrl + C` in your terminal/command prompt.
```

This version includes your requested changes and provides a step-by-step guide for setting up and running the Flask app. Let me know if you need further adjustments!
