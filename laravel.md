# Laravel Cheat Sheet

## Creating a model + migration + controller

```bash
	php artisan make:model Task -mc
```

- Model: Task
- Migration: create_tasks_table
- Controller: TaskController

## Conventions

GET /posts - display all posts

GET /posts/create - show page for creating posts

POST /posts - Publish a post

GET /posts/{id} - show page for 1 post

GET /posts/{id}/edit - show page to edit post

PATCH /posts/{id} - Edit a post

DELETE /posts/{id} - Delete a post
