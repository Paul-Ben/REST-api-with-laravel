# REST-api-with-laravel

### Description:
This is a simple REST API CRUD application using Laravel (laravel version 10).

## How to Use
1. Clone the repository and navigate (cd) into it: `git clone https://github.com/Paul-Ben/REST-api-with-laravel
2. copy contents of .env.example file to .env file.
3. update the database details in the .env file as DB_DATABASE= your_Database_name
DB_USERNAME=your_username
DB_PASSWORD=your_password
4. run the commands: *composer update* and *composer install*
5. Next run the command: *php artisan migrate --seed* to run the database migrations and seed the database with sample data
6. Next run the command: *php artisan serve* to run the server to serve the project.
7. browser url is http://127.0.0.1:8000 to check that the application is running fine.
8. Next open your favourite rest client eg. postman or thunder client etc and test out the api endpoints.

### API EndPoints:
* GET: http://127.0.0.1:8000/api/vi/tasks
Returns all tasks
* POST: http://1270.0.1:8000/api/v1/tasks
Add new task with data {"name":"Task Title"}
* PUT: http://127.0.0.1:8000/api/v1/tasks/{task}
Update existing Task, pass id in place of {task}. Data should be like this {"name":"Updated Task Title"}
* PATCH: http://127.0.0.1:8000/api/v1/tasks/{task}/complete
Mark the task as completed by passing task id in place of {task} Data should be like this {"is_completed": true}
* Delete: http://127.0.0.1:8000/api/v1/tasks/{task}
Remove specific task by passing its id in place of {task}