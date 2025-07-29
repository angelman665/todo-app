# To-Do App

A simple To-Do application to manage your daily tasks.

This project is a full-stack application with a React frontend and two separate backends (Spring Boot and NestJS), all containerized with Docker.

## Tech Stack

*   **Frontend:** [React.js](https://reactjs.org/) (with [TypeScript](https://www.typescriptlang.org/))
*   **Backend #1:** [Java](https://www.java.com/) with [Spring Boot](https://spring.io/projects/spring-boot)
*   **Backend #2:** [Node.js](https://nodejs.org/) with [NestJS](https://nestjs.com/)
*   **Database:** [MySQL](https://www.mysql.com/)
*   **Containerization:** [Docker](https://www.docker.com/) & [Docker Compose](https://docs.docker.com/compose/)

## Project Structure

The repository is structured as a monorepo with the following directories:

```
.
├── backend-nestjs/ # NestJS backend source code
├── backend-spring/ # Spring Boot backend source code
├── frontend/       # React frontend source code
└── docker-compose.yml # Docker Compose configuration
```

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

Make sure you have the following software installed on your machine:

*   [Docker](https://docs.docker.com/get-docker/)
*   [Docker Compose](https://docs.docker.com/compose/install/)

### Installation & Running the App

1.  **Clone the repository:**
    ```sh
    git clone https://your-repository-url.git
    cd todo-app
    ```

2.  **Run the application with Docker Compose:**
    This command will build the images for the frontend and backends, and start all the services.
    ```sh
    docker-compose up -d --build
    ```

## Available Services

Once the application is running, you can access the different services at the following URLs:

| Service         | URL                             |
| --------------- | ------------------------------- |
| Frontend        | `http://localhost:3000`         |
| Spring Backend  | `http://localhost:8080`         |
| NestJS Backend  | `http://localhost:3001`         |
| MySQL Database  | `localhost:3306` (from host)    |

## API Documentation

Each backend provides its own API documentation.

*   **Spring Boot:** The API documentation can be found at `http://localhost:8080/swagger-ui.html` (once implemented).
*   **NestJS:** The API documentation can be found at `http://localhost:3001/api` (once implemented).

## Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3.  Commit your Changes (`git commit -m '''Add some AmazingFeature''')
4.  Push to the Branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.
