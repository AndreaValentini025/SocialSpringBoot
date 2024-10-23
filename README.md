# Project README

Welcome to SocialSpringBoot! This README will guide you through the setup and highlight some key functionalities of the application.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation and Setup](#installation-and-setup)
- [Running the Application](#running-the-application)
- [Functionalities](#functionalities)
- [Accessing the MinIO Dashboard](#accessing-the-minio-dashboard)
- [Available Users](#available-users)

## Prerequisites

- **Java Development Kit (JDK) 21**
- **Apache Maven**
- **Docker and Docker Compose**

## Installation and Setup

1. **Clone the Repository**

   ```bash
   git clone https://github.com/AndreaValentini025/SocialSpringBoot.git
   cd SocialSpringBoot
   ```

2. **Build the Project**

   Navigate to the project directory and run:

   ```bash
   mvn clean package -DskipTests
   ```

   This command cleans the project, compiles the source code, and packages it, skipping the tests.

3. **Start the Application with Docker Compose**

   ```bash
   docker compose up --build -d
   ```

   This command builds and starts all the services defined in the `docker-compose.yml` file in detached mode.

## Running the Application

Once the Docker containers are up and running, the application should be accessible at:

- **Web Application URL:** `http://localhost:7000`

## Functionalities

- **User Authentication:** Secure login and registration system for users.
- **File Storage:** Upload and manage files using the MinIO object storage.
- **User Profiles:** View and edit user profiles, including avatars.
- **Posts and Comments:** Create, view, and delete posts.
- **Interactions:** Like and comment posts.
- **GraphQL:** The main service that handles all the application's functionalities interacts with the User's, Post's, and Interaction's services through GraphQL.

## Accessing the MinIO Dashboard

The MinIO Dashboard allows you to manage the application's object storage.

- **URL:** `http://localhost:9001`
- **Username:** `rootname`
- **Password:** `yourpassword`

After logging in, you can view, upload, and manage the files stored by the application.

## Available Users

For testing purposes, the application comes with pre-configured user accounts:

| Username | Password  |
|----------|-----------|
| user1    | password1 |
| user2    | password2 |
| user3    | password3 |
| user4    | password4 |
| user5    | password5 |
| user6    | password6 |

You can log in using the usernames and passwords provided above, or create a new account.

> **Note:** These accounts are for testing purposes only. Please do not use them in a production environment.

## Support

If you encounter any issues or have questions, feel free to open an issue on the repository or contact me.

---

Thank you for trying out my application!