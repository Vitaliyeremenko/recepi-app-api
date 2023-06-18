# recepi-app-api

Recepi API project

# create project

docker-compose run --rm app sh -c "django-admin startproject app ."

docker-compose run --rm app sh -c "python manage.py startapp core"

# test

docker-compose run --rm app sh -c "python manage.py test"

# create migrations

docker-compose run --rm app sh -c "python manage.py makemigrations"

# run migrations

docker-compose run --rm app sh -c "python manage.py wait_for_db && python manage.py migrate"

# run project

docker-compose up

# -- test user

admin@example.com
