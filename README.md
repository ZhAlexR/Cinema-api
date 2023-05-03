# The Cinema API project

The "Cinema-api" project is an open-source REST API written in DRF, which provides backend support 
for managing cinema-related data such as movies, genres, actors,  showtimes, and reservations. 

It is built using DRF and PostgerSQL, and includes features like authentication, authorization, 
and documentation. 
The project can be used to create, update, delete, and retrieve data through its various endpoints. 
Additionally, it includes automated testing to ensure its functionality.

# API features

- JWT authentication 
- Admin panel at <span style="color: rgb(255, 76, 96);">/admin/<span> 
- API documentation at <span style="color: rgb(255, 76, 96)">/api/doc/swagger/<span> 
- Managing orders and tickets 
- Creation of movies with genres and actors 
- Creation of cinema halls 
- Addition of movie sessions 
- Filtering of movies and movie sessions

# Installation via GitHub

If you don't have PostgreSQL - [install it](https://www.postgresql.org/download/) or use some remote DB such as [Elephant](https://customer.elephantsql.com/)

```shell
git clone git@github.com:ZhAlexR/Cinema-api.git
cd Cinema-api
python3 -m venv venv
source venv/bin/activete # for linux or macOS
venv\Scripts\activete # for Windows
```
>Pay attention! You have to set up ENVIRONMENT VARIABLES!!!

Create `.env` file inside your project root. Use `.env.semple` as template:
```shell
POSTGRES_HOST=POSTGRES_HOST
POSTGRES_NAME=POSTGRES_NAME
POSTGRES_USER=POSTGRES_USER
POSTGRES_PASSWORD=POSTGRES_PASSWORD

DJANGO_SECRET_KEY=DJANGO_SECRET_KEY
DEBUG=DEBUG
ALLOWED_HOSTS=ALLOWED_HOSTS
```
Change the part after `=` to your valid credentials, for example:
`POSTGRES_NAME=your_database_name`


Perform the next commands to create migrations for your DB:
```shell
python manage.py makemigration
python manage.py migrate
```

Start your server using:
```shell
python manage.py runserver
```


# Installation via Docker

If you don't have Docker - [install it](https://docs.docker.com/get-docker/)
```shell
git clone git@github.com:ZhAlexR/Cinema-api.git
cd Cinema-api
docker compose build
docker coppose up
```
# <p style="text-align: center;">Enjoy your Cinema API!</p>

<div align="center">
    <img src="https://media.giphy.com/media/t3sZxY5zS5B0z5zMIz/giphy-downsized-large.gif" alt="">
</div>


