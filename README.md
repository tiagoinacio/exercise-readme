# Dashboard Exercise

## Overview

We have a department store where customers can check in, in order to access
information on the latest collections, get product recommendations, discounts,
and other perks.

You will create a dashboard to monitor customers currently in the
store, showing their profile information so that the shop assistants can have a
more personal interaction with them.

We have already implemented the backend server that will support the dashboard
application. This backend manages the user profile information for customers
currently checked in at the store. It also provides a WebSocket endpoint to get
information of users checking in, in real time.

## Tasks

We have split the development of the dashboard application into the following
feature tasks:

### Task 1 - Overview of checked in users

Show a list of cards corresponding to each checked in user.

Each card should show the user's profile information, if available:

- first and last name
- email
- postal code and city
- country

### Task 2 (optional) - Live update of checked in users

Add cards for newly checked in users in real time, as they enter the store,
using the data stream exposed through the WebSocket endpoint.

## Technical requirements

The dashboard should be a client-side web application, built in React  but feel free to use any
other UI library that you need. Keep in mind that the
solution should be as scalable and maintainable as possible, in order to support
future development.

You should build the application for use in production, but you can use an
existing build/template system if you want. The necessary commands to build and
run the application should be documented.

## Optional

Additionally, you could use `git` for version control with clean and
descriptive commits, using at least one commit for each task.

Feel free to add code comments for clarity, and unit tests for relevant functionality.

### Endpoint documentation

The backend server exposes the following HTTP endpoints:

- GET `/api/users/` Get all users currently checked in

Additionally, it exposes a websocket endpoint at `/ws`, providing real time
streaming of users checking in at the store.

Further information on the expected request and response data formats is
available through a Swagger UI at `/documentation`, which should be opened using
a web browser.

