
# Flask To-Do Application

<center>![Screenshot](/screenshots/)
</center>

This is a simple To-Do list application built with Flask and jQuery. The application allows users to add, delete, and update tasks dynamically without needing to reload the page. It uses AJAX to communicate with the server and update the task list in real time.

## Features

- **Add Task**: Users can add new tasks to the list.
- **Delete Task**: Users can remove tasks from the list.
- **Update Task Status**: Users can mark tasks as completed or incomplete by toggling their status.
- **Real-Time Updates**: The application updates the task list and completion status in real time using AJAX.

## Technologies Used

- **Flask**: A lightweight WSGI web application framework for Python.
- **SQLAlchemy**: An ORM (Object Relational Mapper) for database operations.
- **SQLite**: A lightweight database used to store tasks.
- **HTML/CSS/Bootstrap**: For the front-end design and layout.
- **jQuery**: A JavaScript library used for DOM manipulation and AJAX requests.

## Installation

### Prerequisites

- Python 3.x
- `pip` (Python package installer)

### Setup Instructions

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/flask-todo-app.git
   cd flask-todo-app
   ```

2. **Create a Virtual Environment**

   ```bash
   python -m venv venv
   ```

3. **Activate the Virtual Environment**

   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install the Required Packages**

   ```bash
   pip install -r requirements.txt
   ```

5. **Run the Application**

   ```bash
   python app.py
   ```

6. **Access the Application**

   Open your web browser and go to `http://127.0.0.1:5000/`.

## Usage

- **Adding a Task**: Enter the task description in the input field and click the "Add" button.
- **Deleting a Task**: Click the "Delete Task" button next to the task you want to remove.
- **Updating a Task Status**: Click the "Update Task" button next to the task to mark it as completed or incomplete.
- **Task Completion Summary**: The application shows a summary of completed and total tasks at the top of the task list.


## AJAX Functionality

The application uses AJAX to handle the addition, deletion, and updating of tasks without requiring a full page reload. This improves user experience by making the application more responsive.

### Example AJAX Workflow

1. **Add Task**: When the user submits a new task, an AJAX POST request is sent to the server. The server processes the request, adds the task to the database, and returns a JSON response with the updated task list. The page is then updated dynamically without a reload.

2. **Delete Task**: When the user deletes a task, an AJAX POST request is sent to the server to remove the task from the database. The task is then removed from the DOM.

3. **Update Task Status**: When the user updates a task's status, an AJAX POST request toggles the task's completion status. The task's appearance is updated to reflect its new state.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
