## Django-start using Docker
###### After cloning this repo and before running the necessary migration you can add custom user model as new app.
<br/>

### HOW TO USE:

#### Install docker if it is not installed yet!

#### Download .zip from github to your project folder -> https://github.com/grbeno/Django-docker-start.git

'''$ cd <your_project_folder>
'''

'''$ docker-compose build
'''

'''$ docker-compose up -d
'''

#### Call localhost in your browser to test!

##### * You should generate new secret-key with: $ docker-compose exec web python -c 'import secrets;print(secrets.token_urlsafe(38))'
##### * you should then create <.env> file in the main folder, export new secret-key, then call it as <web:environment:> in your <.yml> file with ${DJANGO_SECRET_KEY}!