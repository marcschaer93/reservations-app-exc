# Reservation App

## Lunchly Reservation System

## Description

Lunchly is an Express app that is *not* an API server, nor is it RESTful.
Instead, it’s a server-side templated application with custom URLs.

## Technologies

    - Express.js, PostgreSQL, nunjucks

- **Setting Up**

  - Set up the `lunchly` database.
  - Connnect to database and fill tables with `data.sql`
  - Start the server with `nodemon`.

## Installation (npm & psql)

```
npm install

createdb lunchly
psql -U <yourusername> -d lunchly -a -f data.sql

npm start

```

- **Exploring the Code**

  - **app.js:** Application object importable from other files/tests.
  - **models/:** Model objects as classes for database handling.
  - **routes.js:** Web interface routes.
  - **server.js:** Functionality to start the server.
  - **templates/:** Nunjucks templates for rendering.

- **Class (Static) Methods**

  - Understanding static methods for class-related functions.
  - Focus on `get(id)` method of the `Customer` class.

- **Nunjucks Templating**

  - Utilizing Nunjucks library for HTML templating.
  - Reviewing templates in `/templates/`.

- **Full Names**

  - Creating a `fullName` function in the `Customer` class.
  - Update templates to refer to the `fullName` function.

- **Saving Reservations**
  - Developing a `.save()` method for reservations.
