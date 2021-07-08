A link to your live application
Screenshots of your application. This makes your application description much easier to understand.
A summary section that concisely explains what your application does. Try to frame this from the standpoint of what the user does, or how the application benefits the user.
Installation instructions

# Capstone: Restaurant Reservation System

This is an application for restaurant employees to keep track of reservations made. It was made using HTML5, CSS3, JavaScript ES6, PostgreSQL, Express.js, React.js, Node.js, and Knex.js.


## API Documentation

| Endpoint | Method | Description |
| ---------------- | -----------------------------------------------| ----------------- |
| /reservations | GET | Retrieves all existing reservations. |
| /reservations | POST | Creates a new reservation. |
| /reservations/:reservation_id | GET | Gets the reservation with specific 'reservation_id'. |
| /reservations/:reservation_id | PUT | Updates the reservation. |
| /reservations/:reservation_id/status | PUT | Updates the reservation status. |
| /tables | GET | Retrieves all existing tables. |
| /tables | POST | Creates a new table. |
| /tables/:tableId/seat | PUT | Assigns a reservation to a table. |
| /tables/:tableId/seat | DELETE | Clears a table for future use. |


### The Application

The application has four main pages: the Dashboard, a search by phone number function, add a new reservation, and add a new table. 

#### The Dashboard 
Also considered the home page, the Dashboard shows the reservations (defaulted for the current date) and the tables. If there are no reservations, a button appears to add one. This is also the page where you can assign reservations to tables.

![Alt text](/path/to/img.jpg "Dashboard")

#### Installation
