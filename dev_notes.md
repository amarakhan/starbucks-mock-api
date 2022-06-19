### DEV NOTES

Make initial migrations for custom models
`docker-compose run --rm app sh -c "python manage.py makemigrations"`

Wait for db and apply migrations to the project
`run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"`

Clear any containers
`docker-compose down`

List docker volumes
`docker volume ls`

Remove volume for db data
`docker volume rm starbucks-mock-api_dev-db-data`