web: newrelic-admin run-program gunicorn -c gunicorn.py.ini wsgi:application
scheduler: python manage.py celery worker -B -E --maxtasksperchild=1000 --loglevel=info
worker: python manage.py celery worker -E --maxtasksperchild=1000
