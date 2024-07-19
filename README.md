# Sri Mandir Clone

This project is a clone of the [Sri Mandir](http://www.srimandir.com/) website, built using React for the frontend and Node.js with SQLite for the backend. The purpose of this project is to replicate the design and functionality of the original website as demonstrated in the provided Loom video.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
  - [Frontend Setup](#frontend-setup)
  - [Backend Setup](#backend-setup)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)

## Features

- Responsive design with React
- Navigation bar with links to Home, Puja, and Booking pages
- Booking form to submit puja requests
- Backend server with Express
- SQLite database for data storage

## Installation

### Frontend Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/dhirajkumar0/srimandir-clone.git
   cd srimandir-clone

   ```

2. Project Structure (fronted)

srimandir-clone/ ├── public/ ├── src/ │ ├── components/ │ │ ├── Navbar.js │ │ ├── Home.js │ │ ├── Puja.js │ │ ├── Booking.js │ ├── App.js │ ├── index.js │ ├── App.css ├── package.json └── ...

backend/ ├── db/ │ └── database.sqlite ├── routes/ │ ├── bookings.js │ ├── pujas.js ├── server.js ├── package.json └── ...

Install the dependencies:

- bash

* Copy code

- npm install

* Start the React development server:

- bash

* Copy code
* npm start

- Backend Setup

* Navigate to the backend directory:

- bash

* Copy code

- cd backend

* Install the dependencies:

- bash

* Copy code

- npm install

* Create the SQLite database and initialize the tables:

- bash

* Copy code
* sqlite3 db/database.sqlite

- Create the bookings table:

- sql

* Copy code CREATE TABLE bookings ( id INTEGER PRIMARY KEY AUTOINCREMENT, name TEXT, email TEXT, puja TEXT );

- Start the Node.js server:

- bash

* Copy code

- node server.js
- Usage

* Ensure both the frontend and backend servers are running.
* Open your browser and navigate to http://localhost:3000 to view the website.
* Use the navigation bar to explore different pages.
* Submit a booking request through the booking form.

- API Endpoints

* Bookings
* POST /api/bookings
* Description: Create a new booking.
* Request Body:

- json Copy code { "name": "John Doe", "email": "john@example.com", "puja": "Puja Name" } Response: json Copy code { "id": 1 }
- Pujas Define additional endpoints for puja services as needed. Deployment Frontend Build the React application:

- bash Copy code npm run build Deploy the build directory to a hosting service like Netlify.

- Backend Deploy the backend server to a platform like Heroku. Ensure the database is properly configured and accessible. Contributing Fork the repository. Create a new branch (git checkout -b feature-branch). Make your changes and commit them (git commit -m 'Add some feature'). Push to the branch (git push origin feature-branch). Open a Pull Request. License This project is licensed under the MIT License.

Feel free to modify the `README.md` to better suit your project's specifics and requirements.
