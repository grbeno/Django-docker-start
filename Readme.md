## Django-docker-start

### How to use:

#### 1. Install docker if it is not installed yet!

#### 2. Download .zip from github to your project folder -> https://github.com/grbeno/Django-docker-start.git

#### 3. Docker commands:

```$ cd <your_project_folder>``` 

```$ docker-compose build```

```$ docker-compose up -d```

#### 4. Open browser and localhost!

##### * You should generate new secret-key with: $ docker-compose exec web python -c 'import secrets;print(secrets.token_urlsafe(38))', you should then create <.env> file in the main folder, export new secret-key, then call it as <web:environment:> in your <.yml> file with ${DJANGO_SECRET_KEY}!