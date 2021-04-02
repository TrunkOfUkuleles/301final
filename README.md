# Code 301 Final Assessment

This assessment comes in 2 parts (applications), a **client** and a **server**

Each application is intended to be operated and tested independently, while also working together.

- The server, written in express, when started, will be the API that the react application uses for data retrieval and storage

## The API Server

Located in the `/server` folder, this is an express server designed to perform CRUD (Create, Read, Update, Delete) operations on a mongo/mongoose data model: `items`. Note that this server does not require you to install or configure MongoDB, it will take care of that for you.

> However, this server is broken. Your task is to fix the bugs.

How will you know that you've found them all? The tests will all pass!

### Server: Running the tests

- Make sure the server is NOT running
- From the root directory of the server in the terminal, run the command `npm test`
- You should recieve a list of the tests that are passing and failing just like you have seen in your code challenges

### Server: Getting Started

- create a repo on GitHub 
- Connect it to your server:
  - run `npm init`
  - run `git remote add origin <repo url>`

- Install your dependencies
- Run the tests
  - with the server turned off run the command: `npm test`
- Fix the bugs - 30 POINTS
- Repeat until all tests are passing
- Deploy to Heroku - 5 POINTS

### Server: Notes

- You may inspect the tests, but do not change them.
- Once you have this working, keep it running. The React app will be using it to save and retrieve data

## The React App

The React application will allow a user to:

- Add a new item
- Add notes to an existing item
- Delete an item from the list

By default, it'll try and connect to your running API server from the previous step to do so.

> However, it's slightly broken and will need you to find and fix it's bugs before you can take on the real challenge.

How will you know that you've found them all? The tests will all pass!

### React App: Getting Started

- create a repo on GitHub
- connect it to your React app:
  - run `git remote add origin <repo url>`

- Install your dependencies
- Run the tests
  - with the React App turned off run `npm test`
- Fix the bugs - 30 POINTS
- Repeat until all tests are passing
- Deploy to Netlify - 5 POINTS

### React App: Add Styling - 30 POINTS

- Using React Bootstrap, style the application in a pleasing and professional way using Bootstrap Components

### React App Notes

- Throughout the application code, you will see that some components/markup have a prop called **data-testid** that look like the below -- **Do not remove or change these, they are required for the tests and grading**
  - ```data-testid="---"```
- When you are running the application and manually testing in the browser, it'll use your server and will not operate unless it is running
- When you are running the tests with `npm test` the application will simulate having a server, so it's not necessary to have it running while doing your pure testing/bug-fixing work

## Rubric

- 30 Points: Fix the Express API Server (all tests passing)
- 30 Points: Fix the React App (all tests passing)
- 30 Points: Style the application (well) with Bootstrap
- 10 Points: Deployed and Tested in the cloud
  - Server running at Heroku
  - React App running at Netlify, configured to talk to the deployed server 
  - Tests for both running in the green at GitHub
