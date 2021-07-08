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

![Alt text](/screenshots/us-06-dashboard-displays-status.png "Dashboard")
#### The Search Function
Navigating to the search function, the user can enter the phone number with which a reservation was set to pull up all records of the reservation associated with that phone number. 

![Alt text](/screenshots/us-07-search-reservations-submit-valid-after.png "Search")
#### New Reservation
This page navigates the user to enter a new reservation. A new reservation includes first name, last name, phone number, the date of the reservation, the time of the reservation, and how many people are included in the reservation. The form also requires users to enter a time that is within restaurant hours. 

![Alt text](/screenshots/us-02-reservation-is-working-day-before.png "new Reservation")
#### New Table
Users have the capability to add a new table with a name and the capacity of that table.

![Alt text](/screenshots/Screenshot%202021-07-08%20160616.png "new Table")
## Installation

1. Clone this repository or download the zip file. 
1. Run `cp ./back-end/.env.sample ./back-end/.env`.
1. Update the `./back-end/.env` file with the connection URL's to your database instances.
1. Run `cp ./front-end/.env.sample ./front-end/.env`.
1. You should not need to make changes to the `./front-end/.env` file unless you want to connect to a backend at a location other than `http://localhost:5000`.
1. Run `npm install` to install project dependencies.
1. Run `npm run start:dev` to start your server in development mode.
