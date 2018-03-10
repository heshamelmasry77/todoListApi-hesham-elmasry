# todoListApi-hesham-elmasry


This is an CRUD app for a Todo List where you can create read update and delete a task.


before anything:

please make sure you have node, express, mongodb and mongoose and nodemon for automating installed
please run ```npm i``` to do that

to run : ```nodemon server```


I used Node Express and mongodb.

The project divided in to three folders:

1.controllers: is where my functions lives :# five(5) different functions namely:  list_all_tasks, create_a_task, read_a_task, update_a_task, delete_a_task.
I exported each of the functions for us to use in the routes.
Each of these functions uses different mongoose methods such as find, findById, findOneAndUpdate, save and remove.

2.models: I required the mongoose in my file and then, I created a model of how my collection should look like.
As you can see, it the task collection(table) will contain a name: a string, and the date it was created. It also contains task status which I have defined as pending - a default value for every task created.

3.routes: # Setting up the routes
Routing refers to determining how an application responds to a client request for a specific endpoint, which is a URI (or path) and a specific HTTP request method (GET, POST, and so on).
Each of my routes has different route handler functions, which are executed when the route is matched.
Below i have defined two basic routes(‘/tasks’, and ‘/tasks/taskId’) with different methods
‘/tasks’ has to methods(‘GET’ and ‘POST’), while ‘/tasks/taskId’ has GET, PUT and DELETE.
As you can see, i required the controller so each of the routes methods can call it’s respective handler function.


thank you
Hesham el masry
