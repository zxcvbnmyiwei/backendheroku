release: python manage.py migrate
celery -A main worker -l info --pool=solo
web: gunicorn main.wsgi:application