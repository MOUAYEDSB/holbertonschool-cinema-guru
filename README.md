# holbertonschool-cinema-guru

<img src="image/redame.avif" alt="Alt Text">


# Pocket Movie App

Welcome to the Pocket Movie App! This app allows users to keep track of their favorite movies and set up a "watch later" list. It is built using React and connects to a backend server to manage authentication and movie data.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Setup and Installation](#setup-and-installation)
- [Project Structure](#project-structure)
- [Components](#components)
  - [General Components](#general-components)
  - [Authentication](#authentication)
  - [Dashboard](#dashboard)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Pocket Movie App is designed to help users organize their movie preferences by allowing them to log in, browse movies, add them to favorites, and create a watch later list.

## Features

- User Authentication (Login/Register)
- Browse and filter movies
- Add movies to favorites
- Create a watch later list
- Responsive design

## Technologies Used

- **Frontend**: React, React Router, React Hooks, Font Awesome
- **Backend**: Node.js, Express, Docker
- **API**: Axios for HTTP requests
- **Styling**: CSS

## Setup and Installation

### Prerequisites

- Docker and Docker Compose
- Yarn package manager

### Backend Setup

1. **Clone the Backend Repository**:
    ```bash
    git clone https://github.com/MOUAYEDSB/holbertonschool-cinema-guru
    cd holbertonschool-cinema-guru
    ```

2. **Build and Run the Backend**:
    ```bash
    docker-compose build --no-cache --force-rm
    docker-compose up
    ```

### Frontend Setup

1. **Create React App**:
    ```bash
    yarn create react-app pocket-movie-app
    cd pocket-movie-app
    ```

2. **Remove Unnecessary Files**:
    - `src/App.test.js`
    - `src/reportWebVitals.js`
    - `src/setupTests.js`
    - `src/logo.svg`

3. **Install Required Packages**:
    ```bash
    yarn add @fortawesome/fontawesome-svg-core @fortawesome/free-solid-svg-icons @fortawesome/react-fontawesome axios lodash normalize.css
    ```

4. **Setup Project Structure**:
    ```
    pocket-movie-app/
    ├── public/
    └── src/
        ├── assets/
        ├── components/
        │   └── general/
        │   └── movies/
        │   └── navigation/
        └── routes/
            └── auth/
            └── dashboard/
    ```

## Project Structure

- `public/`: Public assets
- `src/`: Source code
  - `assets/`: Static assets
  - `components/`: Reusable components
    - `general/`: General UI components like Input, Button, etc.
    - `movies/`: Movie-related components like Tag, Filter, etc.
    - `navigation/`: Navigation components like Header, SideBar, etc.
  - `routes/`: Page components for routing
    - `auth/`: Authentication pages (Login, Register)
    - `dashboard/`: Main dashboard and sub-pages (HomePage, Favorites, WatchLater)

## Components

### General Components

- **Input**: A styled input field with label and icon support.
- **SelectInput**: A dropdown select input.
- **Button**: A styled button with optional icon.
- **SearchBar**: A search input for movie titles.

### Authentication

- **Authentication**: Handles switching between login and register forms.
- **Login**: Login form for user authentication.
- **Register**: Registration form for new users.

### Dashboard

- **Header**: Displays user info and logout option.
- **SideBar**: Navigation sidebar with activity log.
- **HomePage**: Main page to browse and filter movies.
- **Favorites**: Page to view user's favorite movies.
- **WatchLater**: Page to view user's watch later list.

## Usage

1. **Start the Backend**: Ensure Docker is running and start the backend using `docker-compose up`.
2. **Start the Frontend**: In the `pocket-movie-app` directory, run:
    ```bash
    yarn start
    ```
3. **Access the App**: Open `http://localhost:3000` in your browser.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a Pull Request.

## Authors

- [Mouayed sabbagh](https://github.com/MOUAYEDSB)