web: gunicorn app:app --max-requests 500 --preload --timeout 29 --worker-class eventlet
worker: celery worker -A app.celery --loglevel=INFO -P eventlet --concurrency=2 --autoscale=6,2