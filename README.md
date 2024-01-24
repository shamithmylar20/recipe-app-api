# Recipe App API

This is the API for a recipe application. It allows creating, reading, updating, and deleting recipes.

## Features

- Create, read, update, and delete recipes
- Authentication system allowing users to register and log in
- User profiles storing basic user info and their recipes
- Search recipes by title or ingredients
- Filter recipes by tags

## Technical Details

- Built with Django REST Framework
- Uses a PostgreSQL database
- Containerized using Docker for easier deployment
- CI/CD pipelines implemented with GitHub Actions

## Usage

Make sure Docker is installed.

To get started with the Recipe App API, follow the steps below:

1. Clone the repository:

    ```bash
    git clone https://github.com/shamithmylar20/recipe-app-api.git
    ```

2. Navigate to the project directory:

    ```bash
    cd recipe-app-api
    ```

3. Build the Docker image:

    ```bash
    docker-compose build
    ```

4. Run the containers:

    ```bash
    docker-compose up
    ```

The API will now be accessible at [http://localhost:8000](http://localhost:8000).

The admin panel can be accessed at [http://localhost:8000/admin](http://localhost:8000/admin).

## Tutorial

[![How to Create Token And Authenticate](https://imgur.com/a/jXUq2UZ)](https://youtu.be/hAN9F2IqGp4)


## API Endpoints

### Recipe Ingredients

- **GET** `/api/recipe/ingredients/`
- **PUT** `/api/recipe/ingredients/{id}/`
- **PATCH** `/api/recipe/ingredients/{id}/`
- **DELETE** `/api/recipe/ingredients/{id}/`

### Recipe Recipes

- **GET** `/api/recipe/recipes/`
- **POST** `/api/recipe/recipes/`
- **GET** `/api/recipe/recipes/{id}/`
- **PUT** `/api/recipe/recipes/{id}/`
- **PATCH** `/api/recipe/recipes/{id}/`
- **DELETE** `/api/recipe/recipes/{id}/`
- **POST** `/api/recipe/recipes/{id}/upload-image/`

### Recipe Tags

- **GET** `/api/recipe/tags/`
- **PUT** `/api/recipe/tags/{id}/`
- **PATCH** `/api/recipe/tags/{id}/`
- **DELETE** `/api/recipe/tags/{id}/`

### Schema

- **GET** `/api/schema/`

### User

- **POST** `/api/user/create/`
- **GET** `/api/user/me/`
- **PUT** `/api/user/me/`
- **PATCH** `/api/user/me/`
- **POST** `/api/user/token/`
