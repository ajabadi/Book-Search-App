# Book-Search-App

## Overview

This week's challenge is about evolving a fully functioning Google Books API search engine built with a RESTful API into a more modern architecture using GraphQL. The original application, developed with the MERN stack (MongoDB, Express.js, React, and Node.js), enables users to save their book searches. Your task is to refactor this application to leverage GraphQL with Apollo Server for data fetching and mutations, enhancing performance and meeting the modern demands of web development.


## Installations

- Node.js
- MongoDB


## Objectives

Refactor the API: Transition from a RESTful API to a GraphQL API using Apollo Server.
Update Authentication Middleware: Ensure the existing authentication works with GraphQL.
Integrate Apollo Provider: Enable frontend communication with Apollo Server.
Deployment: Launch the application on Render.
Getting Started

## User Story
As an avid reader, I want to search for new books to read so that I can keep a list of books to purchase.

## Acceptance Criteria
Upon loading, the app presents a menu with "Search for Books" and "Login/Signup" options, an input field for searches, and a submit button.
The "Search for Books" option allows users to input a search term and submit it.
Non-logged-in users can search for books and see results with titles, authors, descriptions, images, and links to the Google Books site.
The "Login/Signup" option opens a modal for user authentication.
Logged-in users can save books to their account and view them on a "Saved Books" page.
Users can remove books from their saved list.
Logging out returns the user to the non-authenticated state of the app.

The app allows users to search for books, save them, and view their saved books in a dedicated page.

## Implementation Details

 - Back-End Specifications
auth.js: Update to support GraphQL API.
server.js: Implement Apollo Server as middleware.

- Schemas:
index.js: Export typeDefs and resolvers.
resolvers.js: Define queries and mutations for Mongoose models.
typeDefs.js: Define Query, Mutation, User, Book, and Auth types.

- Front-End Specifications
queries.js: Contains GET_ME query for Apollo Server.
mutations.js: Contains mutations for user login, user addition, book saving, and book removal.
App.jsx: Implement Apollo Provider.
SearchBooks.jsx: Use SAVE_BOOK mutation with useMutation() Hook.
SavedBooks.jsx: Use GET_ME query with useQuery() Hook and REMOVE_BOOK mutation.
SignupForm.jsx and LoginForm.jsx: Use corresponding mutations for user actions.

## Usage

Terimanl: 
- npm install
- cd client
- npm start

## Deployment
Deployed app in on the process

<img width="1307" alt="Screen Shot 2024-03-01 at 21 22 18" src="https://github.com/ajabadi/Book-Search-App/assets/145517793/cfab5e46-8ec6-4783-97a2-1f4a9206faec">

