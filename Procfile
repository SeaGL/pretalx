release: ./src/manage.py migrate
web: gunicorn pretalx.wsgi --chdir src --name pretalx --max-requests 1200  --max-requests-jitter 50 --log-level=info
celery: env -C src/ celery -A pretalx.celery_app worker -l info
