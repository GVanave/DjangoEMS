# DjangoEMS: Company Employee Management System (EMS) using Django REST Framework

DjangoEMS is a basic example of an Employee Management System (EMS) implemented with Django and Django REST Framework.

## Getting Started

1. **Create Virtual Environment:** 
   - Create a virtual environment using:
     ```
     virtualenv name_of_env
     ```
   - Activate the virtual environment:
     ```
     name_of_env/Scripts/activate.ps1
     ```

2. **Install Dependencies:**
   - Install Django and Django REST Framework:
     ```
     pip install django djangorestframework
     ```

3. **Start Project:**
   - Create a new Django project:
     ```
     django-admin startproject name_of_project
     ```
   - Change to the project directory:
     ```
     cd name_of_project
     ```
   - Create a new app within the project:
     ```
     python manage.py startapp name_of_app
     ```

4. **Configure Settings:**
   - Add the newly created app and 'rest_framework' to the `INSTALLED_APPS` in `settings.py`.

5. **Database Migration:**
   - Perform database migrations:
     ```
     python manage.py makemigrations
     python manage.py migrate
     ```

6. **Create Superuser:**
   - Create a superuser for administrative access:
     ```
     python manage.py createsuperuser
     ```

7. **Run Server:**
   - Start the development server:
     ```
     python manage.py runserver
     ```

## Key Components

### Models
- Defined in `models.py`, consisting of three models: Teams, Employees, and Work_Arrangement.

### Serializers
- Defined in `serializer.py`, responsible for converting data types to JSON and vice versa.

### Views
- Defined in `views.py`, including API views for GET, POST, PUT, and DELETE operations.

### URLs
- Defined in `urls.py` of the project, mapping to corresponding views.

### Admin Interface
- Register models in `admin.py` to manage data through Django's admin interface.

## Additional Features

- **Serializer:** Converts data types to JSON and vice versa, facilitating communication between frontend and backend.
- **API Views:** Define operations such as GET, POST, PUT, and DELETE for interacting with the database.
- **Testing:** Utilize `test.py` for testing Django REST functionality.

## Testing the API

- Use `test.py` to perform tests on the Django REST API.
- Run tests using:
