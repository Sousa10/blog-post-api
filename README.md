# Blog Post REST API

This project is a REST API for managing blog posts, created using Django and Django REST Framework.

Features

- Create, read, update, and delete blog posts
- List all blog posts
- Retrieve details of a single blog post

## Requirements

- Python 3.8+
- Django 3.2+
- Django REST Framework 3.12+

## Setup

1. Clone the repository

```sh
git clone [https://github.com/yourusername/blogpost-api.git](https://github.com/Sousa10/blog-post-api.git)
cd blogpost-api
```

2. Create a virtual environment

python -m venv venv

3. Activate the virtual environment

On Windows:
venv\Scripts\activate

On macOS and Linux:
source venv/bin/activate

4. Install the required packages

pip install -r requirements.txt

5. Apply migrations

python manage.py migrate

6. Create a superuser

python manage.py createsuperuser

7. Run the server

python manage.py runserver

The API will be available at http://127.0.0.1:8000/.

# API Endpoints

## List all blog posts

GET /blogposts/

## Create a new blog post

POST /blogposts/

Request body:

{
  "title": "Post Title",
  "content": "Post content"
}

## Retrieve a single blog post

GET /blogposts/{id}/

## Update a blog post

PUT /blogposts/{id}/

Request body:

{
  "title": "Updated Title",
  "content": "Updated content"
}

## Partially update a blog post

PATCH /blogposts/{id}/

Request body:

{
  "title": "Updated Title"
}

## Delete a blog post

DELETE /blogposts/{id}/

