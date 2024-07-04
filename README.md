# Star Wars Web Application

This project is a web application that displays information about Star Wars people and planets using data from the SWAPI (https://swapi.dev/). 

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Application](#running-the-application)

## Features

- Display information about Star Wars people and planets
- Paginated tables with 15 or 30 items per page
- Input search for both people and planets
- Sort functionality for name(string) and created(Date) columns
- Deployed using Docker

## Technologies Used

- **Frontend:** Angular
- **Backend:** Spring Boot
- **Containerization:** Docker, Docker Compose

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- [Angular CLI](https://angular.io/cli)
- [Java JDK 17+](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/<your-username>/star-wars-project.git
    cd star-wars-test
    ```

2. **Backend Setup:**

    - Navigate to the backend directory:

        ```bash
        cd backend
        ```

    - Build the Spring Boot application:

        ```bash
        mvn clean package
        ```

3. **Frontend Setup:**
    - Build the Angular application:

        ```bash
        cd ../front/star-wars-frontend
        ng build star-wars-frontend --configuration production
        ```

## Running the Application

To run the application, use Docker Compose:

1. **Navigate to the root directory:**

    ```bash
    cd ../../
    ```

2. **Run Docker Compose:**

    ```bash
    cd star-wars-test
    docker-compose down && docker-compose build --no-cache && docker-compose up
    ```

3. **Access the Application:**

    Open your web browser and go to `http://localhost:6969`.