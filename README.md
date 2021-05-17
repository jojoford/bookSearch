# Book Search Engine 
## Description
Challenge 21 MERN : Take a fully functioning Google Books API search engine built with a RESTful API, and refactor it to be a GraphQL API built with Apollo Server. The app was built using the MERN stack, with a React front end, MongoDB database, and Node.js/Express.js server and API. It's already set up to allow users to save book searches to the back end.

To fulfill the Challenge, do the following:

Set up an Apollo Server to use GraphQL queries and mutations to fetch and modify data, replacing the existing RESTful API.

Modify the existing authentication middleware so that it works in the context of a GraphQL API.

Create an Apollo Provider so that requests can communicate with an Apollo Server.

Deploy the application to Heroku. [click me!](https://pure-refuge-64079.herokuapp.com/)

## Built With
Apollo

GraphQL

React

## Backend specs
Completed the following tasks in each of these back-end files:

server.js: Implement the Apollo Server and apply it to the Express server as middleware.

auth.js: Update the auth middleware function to work with the GraphQL API.

## Front-End Specs
 Created the following front-end files:

queries.js: This will hold the query GET_ME, which will execute the me query set up using Apollo Server.

mutations.js:

LOGIN_USER will execute the loginUser mutation set up using Apollo Server.

ADD_USER will execute the addUser mutation.

SAVE_BOOK will execute the saveBook mutation.

REMOVE_BOOK will execute the removeBook mutation.

Additionally, you’ll need to complete the following tasks in each of these front-end files:

App.js: Create an Apollo Provider to make every request work with the Apollo server.

SearchBooks.js:

Use the Apollo useMutation() Hook to execute the SAVE_BOOK mutation in the handleSaveBook() function instead of the saveBook() function imported from the API file.

Make sure you keep the logic for saving the book's ID to state in the try...catch block!

SavedBooks.js:

Remove the useEffect() Hook that sets the state for UserData.

Instead, use the useQuery() Hook to execute the GET_ME query on load and save it to a variable named userData.

Use the useMutation() Hook to execute the REMOVE_BOOK mutation in the handleDeleteBook() function instead of the deleteBook() function that's imported from API file. (Make sure you keep the removeBookId() function in place!)

SignupForm.js: Replace the addUser() functionality imported from the API file with the ADD_USER mutation functionality.

LoginForm.js: Replace the loginUser() functionality imported from the API file with the LOGIN_USER mutation functionality.

## screenshot
[![screenshot-mern-21.jpg](https://i.postimg.cc/x1p1bbyC/screenshot-mern-21.jpg)](https://postimg.cc/PCZjgJ7s)



## Contributing

jcgom3 and ortizjavier10

