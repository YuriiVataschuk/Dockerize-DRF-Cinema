# Cinema API

Api service for cinema management written on DRF

## Installing using GitHub

1. Install PostgresSQP and create a database.

2. Clone the repository:

git clone https://github.com/YuriiVataschuk/Dockerize-DRF-Cinema.git
cd py-dockerize-cinema

3. Set up a virtual environment and activate it:

python -m venv venv
source venv/bin/activate

4. Install the required dependencies:

pip install -r requirements.txt

5. Set the following environment variables:

set DB_HOST=<your db hostname>
set DB_NAME=<your db name>
set DB_USER=<your db username>
set DB_PASSWORD=<your db user password>
set SECRET_KEY=<your secret key>

6. Apply database migrations:

python manage.py migrate

7. Start the server:

python manage.py runserver

## Run with Docker

Make sure Docker is installed on your system.

1. Build the Docker image:

docker-compose build

2. Start the containers:
  
docker-compose up

## Getting access

To get access to the API:

- Create a user via `/api/user/register/`.
- Obtain an access token via `/api/user/token/`.

## Features

- JWT authentication
- Admin panel: `/admin/`
- Documentation is located at `/api/doc/swagger/`
- Managing orders and tickets
- Creating movies with genres and actors
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions
