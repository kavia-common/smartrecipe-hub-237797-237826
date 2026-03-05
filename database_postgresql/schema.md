# SmartRecipe Hub - Database Schema

This project uses PostgreSQL. The backend (`backend_fastapi`) manages schema via Alembic migrations.

Core tables:

- `users` (role: `user`|`admin`)
- `recipes`
- `favorites` (user_id, recipe_id)
- `shopping_lists`
- `meal_plans`

To apply schema:
- Run Alembic migrations from the backend container.
