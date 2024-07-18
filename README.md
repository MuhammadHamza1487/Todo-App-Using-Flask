
# Flask Task App

This is a simple task management application built with Flask and SQLAlchemy. It allows users to add, update, and delete tasks. The app uses SQLite as its database.

## Features

- Add new tasks
- View all tasks
- Update existing tasks
- Delete tasks

## Technologies Used

- Python
- Flask
- SQLAlchemy
- SQLite
- Bootstrap

## Project Structure

```plaintext
flask_app/
│
├── instance/
│   └── test.db
├── static/
│   └── css/
│       └── main.css
├── templates/
│   ├── base.html
│   ├── index.html
│   └── update.html
├── venv/
├── app.py
└── create_db.py
```

## Setup Instructions

1. **Clone the repository**
   ```sh
   git clone https://github.com/MuhammadHamza1487/Todo-App-Using-Flask.git
   cd flask-task-app
   ```

2. **Create and activate a virtual environment**
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. **Install the required dependencies**
   ```sh
   pip install Flask Flask-SQLAlchemy
   ```

4. **Create the SQLite database**
   ```sh
   python create_db.py
   ```

5. **Run the application**
   ```sh
   python app.py
   ```

6. **Open your browser and visit**
   ```sh
   http://127.0.0.1:5000
   ```

## File Descriptions

- **app.py**: The main Flask application file containing routes and logic.
- **create_db.py**: Script to create the SQLite database.
- **templates/**: Directory containing HTML templates.
  - **base.html**: Base template extended by other templates.
  - **index.html**: Template for displaying and adding tasks.
  - **update.html**: Template for updating tasks.
- **static/css/main.css**: Custom CSS for styling the application.
- **instance/**: Directory containing the SQLite database.

## Routes

- **/**: Home page where you can view, add, and delete tasks.
- **/delete/<int:id>**: Route to delete a task.
- **/update/<int:id>**: Route to update a task.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any changes.
