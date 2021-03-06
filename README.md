# Power Play Recruiting
This project is a website and system for parents of youth hockey players and young adult hockey players under the age of 21 to showcase themselves to schools, coaches, and other recruiters.  Player accounts will not be able to view or initiate contact with coaches or teams and they will not be able to view other player accounts. Coaches/recruiters will be invited by the Admin user (Mike Bowman, Logan Sharp, Austin Hill). Coaches/recruiters can view active player profiles.

## Prerequisites

Before you get started, make sure you have the following software installed on your computer:

- [Node.js](https://nodejs.org/en/)
- [PostrgeSQL](https://www.postgresql.org/)
- [Nodemon](https://nodemon.io/)

## Create database and table

Download the repository.

Create a new database called `ppr_hockey` and run the SQL queries in the database.sql file

If you would like to name your database something else, you will need to change `ppr_hockey` to the name of your new database name in `server/modules/pool.js`

## Development Setup Instructions

* Run `npm install`
* Create a `.env` file at the root of the project and paste this line into the file:
    ```
    SERVER_SESSION_SECRET=**secret goes here**
    ```
    While you're in the `.env` file, replace `**secret goes here**` with some long random string like `25POUbVtx6RKVNWszd9ERB9Bb6` to keep your application secure. Here's a site that can help you: [https://passwordsgenerator.net/](https://passwordsgenerator.net/). If you don't do this step, create a secret with less than eight characters, or leave it as `superDuperSecret`, you will get a warning.
* Start postgres if not running already by using `brew services start postgresql`
* Run `npm run server`
* Run `npm run client`
* Navigate to `localhost:3000`
