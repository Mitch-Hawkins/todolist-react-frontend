# To-Do List App - React Typescript Frontend

<!-- {add test badges here, all projects you build from here on out will have tests, therefore you should have github workflow badges at the top of your repositories: [Github Workflow Badges](https://docs.github.com/en/actions/monitoring-and-troubleshooting-workflows/adding-a-workflow-status-badge)} -->

## Demo & Snippets

- This app is hosted as a Static Web App using Microsoft Azure, alongside the app's backend services as well as the database.
- https://nice-coast-0ffb54e00.5.azurestaticapps.net

- An Example of an empty to-do list
- ![alt text](<screenshots/Screenshot 2024-03-21 at 10.40.18 am.png>)

- An Example of a to-do list with a few simple tasks and their information
- ![alt text](<screenshots/Screenshot 2024-03-21 at 10.40.23 am.png>)

- Screenshot of what the Create Task modal looks like to the user, where they can input their information
- ![alt text](<screenshots/Screenshot 2024-03-21 at 10.40.53 am.png>)

---

## Requirements / Purpose

- Create a backend with Spring that can create, update, read and delete todos from a MySQL database. Along with this create a frontend application with React that interacts with this backend
- This project is my first foray into building a Full-Stack application. I've created apps that use React frontends before, however this was a fantastic opportunity to combine both my skills of Front end and Back end development together.
- The front end was built using React Typescript. I've made front ends and UI's with React before, but this was my first time incorporating it with Typescript. I find Typescript to work better with incorporating back ends in Java.

---

## Build Steps

- To build, first download the project files. Then, navigate to the directory that the project is located in, and run the following command

```
npm run dev
```

- Once the command has been run, navigate to the url that the app is being hosted on. By default, it should be https://localhost:5173

---

## Design Goals / Approach

- With this front end, I wanted to design a UI with a coherent theme and palette. One of my weaknesses as a developer is aesthetic and balanced design and placement of elements in a UI. I wanted this app to look good on multiple screen sizes and devices.
- Whilst the concept of this app is quite simple in a real-world use context, i still wanted to use clean coding practices, including using contexts where neccessary instead of prop drilling, as well as having organised and well thought out components that are easy to scale and change in the future.

---

## Features

- Can create, read, edit, and delete a dynamic list of To-Do Tasks. Tasks contain the following:
- Name of the task
- A brief description of the task
- Due date for the task
- A priority value for the task (eg. Urgent, Low Priority, etc)
- Contains a UI that works both on Mobile and Desktop
- Connects to a SpringBoot Java backend that processes all the services and stores the tasks in a MySQL database

---

## Known issues

- Error handling is semi-implemented, The errors will appear in the console, however no user-feedback solution has been implemented yet.
- As the modal used for creating and updating tasks uses the recently implemented dialog tag, certain tests have not implemented methods for recognising the different states of this tag. Currently, options are to exclude tests for this tag, or re work the modal in the future to work with different tags.

---

## Future Goals

- Given more time, I would love to implement more error handling, especially with providing user feedback through the idea of using a toast notification universally to let the user know when a task has been successfully created/modified, or if the service was unsuccessful in completion
- Id also love to be more thorough with my testing, as this is something that adds code security as well as forcing my code to be more scaleabe down the line.

---

## Struggles

- Struggled with my first attempt at proper error handling, including working with a GlobalExceptionHandler, as well as working with creating custom exceptions. In the end, I seemed to be fighting with Springs own well thought out exception classes for things such as validation, etc. Certain exceptions that spring does not take care of for example, out of bounds exceptions, I attempted to create exceptions for myself. I have since learned an error handling pattern that I'm comfortabe with, and will look to implement this in the future.

---

## Further details, related projects, reimplementations

- This project connects with my todolist-spring-backend repository, the link to which is here

- https://github.com/Mitch-Hawkins/todolist-spring-backend
