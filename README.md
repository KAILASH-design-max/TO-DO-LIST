A backend application for managing to-do tasks, built using Django and Django Rest Framework (DRF). This application provides RESTful APIs to perform CRUD (Create, Read, Update, Delete) operations on tasks.

Features
Task Management: Create, read, update, and delete tasks.
Django Admin: Manage tasks with a user-friendly admin interface.
Status Management: Supports multiple statuses like OPEN, WORKING, COMPLETED, and more.
Authentication: Basic authentication for secure API access.
API Documentation: Test and explore the APIs using Postman or other tools.
Requirements
Python 3.10 or later
Django 4.2 or later
Django Rest Framework 3.14 or later
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/KAILASH-design-max/TO-DO-LIST?tab=readme-ov-file
cd django-todo-backend
Create a virtual environment:

bash
Copy code
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Run database migrations:

bash
Copy code
python manage.py migrate
Create a superuser (admin):

bash
Copy code
python manage.py createsuperuser
Start the development server:

bash
Copy code
python manage.py runserver
The app will be available at:

arduino
Copy code
 http://127.0.0.1:8000/todos/
API Endpoints
Base URL:
arduino
Copy code
 http://127.0.0.1:8000/todos/
HTTP Method	Endpoint	Description	Request Body
POST	/tasks/create	Create a new task	{ "title": "Task Title", "description": "Task Description", "due_date": "YYYY-MM-DD", "tags": "tag1,tag2" }
GET	/tasks	Retrieve all tasks	None
GET	/tasks/<id>	Retrieve a task by ID	None
PUT	/tasks/update/<id>	Update a task by ID	{ "title": "New Title", "description": "Updated Description", "status": "COMPLETED" }
DELETE	/tasks/delete/<id>	Delete a task by ID	None
Django Admin Panel
You can manage tasks directly via the Django admin interface.

Visit: http://127.0.0.1:8000/todos/
Log in with the superuser credentials you created earlier.



https://github.com/user-attachments/assets/94fa0bfb-ea79-4726-bad9-fc0a914976d7


