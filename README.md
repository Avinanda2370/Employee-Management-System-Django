**Employee Management System**
_Project Overview :-_ 
This is a simple web application built with Django that facilitates employee management. It allows users to perform various operations like viewing all employees, adding new employees, searching for employees, and removing employees.

**Function Overview** 
_hey(request)_
This function renders the index.html template, serving as the homepage or landing page of the application.

_all_emp(request)_
This function retrieves all employee objects from the database using the Employee.objects.all() method.
It passes the retrieved employees to the view_all.html template for display.

_add(request)_
This function handles both GET and POST requests for adding a new employee.
If the request method is POST, it validates the form data submitted by the user and saves the new employee to the database.
If the request method is GET or the form data is invalid, it renders the add_emp.html template with an empty form.

_remove(request, id=0)_
This function handles both GET and POST requests for removing an employee.
If an employee ID is provided in the URL, it attempts to retrieve and delete the corresponding employee from the database.
If no ID is provided or the provided ID is invalid, it retrieves all employees and renders the remove_emp.html template with the list of employees.

_filter(request)_
This function handles both GET and POST requests for filtering employees based on specified criteria (name, department, role).
If the request method is POST, it retrieves the filter criteria from the form data, filters the employee queryset accordingly, and renders the view_all.html template with the filtered results.
If the request method is GET, it renders the filter.html template with the form for entering filter criteria.
If the request method is neither POST nor GET, it returns an error HttpResponse.
These functions collectively provide the core functionality of your Employee Management System, including viewing, adding, removing, and filtering employees.

**Usage**
Clone the repository. 
Install the necessary dependencies using pip `install -r requirements.txt. `
Set up your database configurations in settings.py. 
Run migrations using `python manage.py migrate`. Create a superuser using `python manage.py createsuperuse`r to access the admin panel. 
Populate the database with your personal information, skills, experiences, and clients through the Django admin interface or programmatically. 
Customize templates and stylesheets according to your preferences to personalize the portfolio website. 
Run the development server using python manage.py runserver and navigate to `http://localhost:8000` to view the website.

**Contributing**
Contributions to the project are welcome! If you find any bugs or have suggestions for improvements, please open an issue or submit a pull request on the project repository.

**License**
The news website is open-source software released under the MIT License. Feel free to use, modify, and distribute the code as needed.
![Screenshot (350)](https://github.com/Avinanda2370/Employee-Management-System-Django/assets/102664151/c05bfbe5-815e-4e54-90a2-70ced2d2231e)
![Screenshot (351)](https://github.com/Avinanda2370/Employee-Management-System-Django/assets/102664151/3db70a52-c16a-4d29-8ba8-7e29741529a0)
![Screenshot (352)](https://github.com/Avinanda2370/Employee-Management-System-Django/assets/102664151/c00711b0-6985-4d8c-a3e2-fcd8512265fd)
![Screenshot (349)](https://github.com/Avinanda2370/Employee-Management-System-Django/assets/102664151/be35b2cd-bcb7-4121-8be2-05d659e467da)

