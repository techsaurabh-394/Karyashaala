# KaryaShaala

KaryaShaala is a web portal designed using React, Bootstrap, and NodeJS that provides details of upcoming academic activities such as conferences, seminars, educational sessions, and other tech or academic events conducted in different colleges. Students can check all these activities, and organizers can register their events.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Event Listings:** View upcoming conferences, seminars, educational sessions, and other academic events.
- **Event Registration:** Organizers can register and manage their events.
- **User Authentication:** Secure user authentication for students and event organizers.
- **Responsive Design:** Fully responsive design using Bootstrap.
- **Real-time Updates:** Real-time updates on event details.

## Technologies Used

- **Frontend:**
  - React
  - Bootstrap

- **Backend:**
  - NodeJS
  - Express
  - MongoDB

- **Other:**
  - JWT for authentication
  - Axios for API calls
  - Mongoose for MongoDB interaction

## Installation

Follow these steps to set up the project locally:

### Prerequisites

- Node.js installed on your machine
- MongoDB instance running

### Steps

1. **Clone the repository:**
    ```sh
    git clone https://github.com/your-username/karyashaala.git
    cd karyashaala
    ```

2. **Install dependencies:**
    ```sh
    npm install
    cd client
    npm install
    ```

3. **Set up environment variables:**
    Create a `.env` file in the root directory and add the following:
    ```sh
    MONGO_URI=your-mongodb-uri
    JWT_SECRET=your-jwt-secret
    ```

4. **Run the server:**
    ```sh
    npm run server
    ```

5. **Run the client:**
    Open another terminal window, navigate to the `client` directory, and run:
    ```sh
    npm start
    ```

The application will be running on `http://localhost:3000` for the frontend and `http://localhost:5000` for the backend.

## Usage

### Registering as an Organizer

1. Click on the "Register" button on the homepage.
2. Fill out the registration form with your details.
3. Once registered, log in to your account.
4. Navigate to the "Add Event" section to register a new event.

### Viewing Events as a Student

1. Navigate to the homepage.
2. Browse the list of upcoming events.
3. Click on any event to view more details.

## API Endpoints

### Authentication

- **POST /api/auth/register**
  - Register a new user.

- **POST /api/auth/login**
  - Log in a user.

### Events

- **GET /api/events**
  - Get a list of all events.

- **POST /api/events**
  - Create a new event (organizers only).

- **GET /api/events/:id**
  - Get details of a specific event.

- **PUT /api/events/:id**
  - Update an event (organizers only).

- **DELETE /api/events/:id**
  - Delete an event (organizers only).

## Contributing

We welcome contributions to KaryaShaala! Here's how you can help:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add some feature'`).
5. Push to the branch (`git push origin feature/your-feature-name`).
6. Open a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to customize this documentation to better fit your project's needs.
