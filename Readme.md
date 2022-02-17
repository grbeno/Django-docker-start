## Django-docker-start

### How to use:

#### 1. Install docker if it is not installed yet

#### 2. Download .zip from github to your project folder

```$ cd <your_project_folder>```

#### 3. Run docker commands: 

```$ docker-compose build```

```$ docker-compose up -d```

##### You can also migrate your data within docker:

```$ docker-compose exec web python manage.py migrate```

#### 4. Open browser and localhost!

##### You should generate new secret-key with:

```$ docker-compose exec web python -c 'import secrets;print(secrets.token_urlsafe(38))'```

##### You should then create .env file in the project folder, export new secret-key, then call it as in ( web: -> environment: ) - already set in your .yml file with ${DJANGO_SECRET_KEY}!