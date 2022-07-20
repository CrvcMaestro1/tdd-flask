# Flask TDD

## Environment variables
```
set FLASK_ENV=development
set FLASK_CONFIG=development
```
## Commands
### Run without docker
```
python manage.py flask run
```
### Run with docker
```
python manage.py compose up -d
```
### Stop
```
python manage.py compose down 
```
### Explore in container bash
```
python manage.py compose exec web bash
```
### Database initialisation (in web bash)
```
python manage.py flask db init
```
### Database migrate and upgrade (in web bash)
```
python manage.py flask db migrate
python manage.py flask db upgrade
```
### Explore database 
```
python manage.py compose exec db psql -U postgres
```