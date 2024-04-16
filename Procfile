web: gunicorn pretalx.wsgi  --name pretalx --max-requests 1200  --max-requests-jitter 50 --log-level=info --bind=127.0.0.1:8345
celery: celery -A pretalx.celery_app worker -l info
