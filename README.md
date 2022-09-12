# Dockerized Cinema API

DRF API service for cinema management

## Installing using Github

```shell
git clone https://github.com/DanRoman-code/dokerize-cinema-api.git
python3 -m venv venv
source venv/bin/activate (on Linux and macOS) or venv\Scripts\activate (on Windows)
pip install -r requirements.txt
set DB_HOST=<your db hostname>
set DB_NAME=<your db name>
set DB_USER=<your db username>
set DB_PASSWORD=<your db user password>
set SECRET_KEY=<your secret key>
python manage.py runmigtarions
python manage.py runserver
```
### Run with docker

```shell
docker-compose build
docker-compose up
```

Getting access
-
- create user via /api/user/register/
- get access token via /api/user/token/


Features
-
- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres, actors and image
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions
