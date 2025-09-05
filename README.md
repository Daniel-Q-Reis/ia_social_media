# IA Social Media 🚀

![Status: In Development](https://img.shields.io/badge/status-in--development-yellow)
![Language](https://img.shields.io/badge/language-Go-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green)

## 📖 About The Project

**IA Social Media** is a learning and portfolio project that explores the evolution and refactoring of a RESTful API for a social network. The original project, a functional Go API, serves as a foundation for a continuous improvement process, leveraging **Artificial Intelligence as an assistive tool** to optimize architecture, enhance code quality, and implement new features.

The goal is to create a full-stack application, documenting the journey of transforming a functional piece of software into a robust, scalable, and modern application.

## 🏛️ Project Structure

The project is organized in a monorepo structure, containing two main applications:

-   **/api**: The application's backend, a RESTful API developed in Go that handles all business logic, users, authentication, and posts.
-   **/webapp**: The application's frontend, which will consume the data from the `/api` to provide an interactive user interface. (To be developed in the future).

## ✨ Key Features

### API (Backend)

-   [x] Full User CRUD
-   [x] User authentication with JWT
-   [x] Full Posts CRUD
-   [x] Follow/Unfollow user system
-   [x] Like/Unlike posts system
-   [🚧] **In Development:** User profile picture uploads
-   [💡] **Planned:** Comments on posts

## 🛠️ Tech Stack

### Backend (`/api`)

-   **Language:** [Go](https://golang.org/)
-   **Router:** [Gorilla/Mux](https://github.com/gorilla/mux)
-   **Database:** [MySQL](https://www.mysql.com/)
-   **Authentication:** [JWT (JSON Web Tokens)](https://jwt.io/)
-   **Environment Variables:** [GoDotEnv](https://github.com/joho/godotenv)

### Frontend (`/webapp`)

-   *(To be defined - e.g., React, Vue, Angular)*

## 🚀 Getting Started (API)

To get the backend up and running on your local machine, follow these steps.

### Prerequisites

-   [Go](https://golang.org/dl/) (version 1.18 or higher)
-   [MySQL](https://dev.mysql.com/downloads/installer/) or [Docker](https://www.docker.com/) with a MySQL image
-   An API client, such as [Postman](https://www.postman.com/) or [Insomnia](https://insomnia.rest/)

### Installation & Running

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR-USERNAME/ia_social_media.git](https://github.com/YOUR-USERNAME/ia_social_media.git)
    cd ia_social_media/api
    ```

2.  **Set up environment variables:**
    -   Rename the `.env.example` file to `.env`.
    -   Open the `.env` file and fill in your database credentials and a `SECRET_KEY` for JWT.
    ```env
    API_PORT=5000
    DB_USER=root
    DB_PASSWORD=your_password_here
    DB_NAME=iasocialmedia
    SECRET_KEY=your_super_secret_key_here
    ```

3.  **Create the database and tables:**
    -   Run the SQL scripts located in the `/api/sql` folder in your MySQL database to create the required tables.

4.  **Install dependencies and run the API:**
    ```bash
    go mod tidy
    go run main.go
    ```

5.  You're all set! The API will be running on `http://localhost:5000`.

## 🤝 Contributing

This is a learning project, but contributions and suggestions are always welcome! If you find a bug or have an idea, feel free to open an *Issue*.

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---
Made with ❤️ and a lot of code!