FROM python:3

LABEL maintainer="ywkim@illinois.edu"

WORKDIR /app
COPY auth-middleware-test-svc /app/
COPY lib /lib/
RUN pip install -r /app/requirements.txt

CMD ["gunicorn", "flaskapp:app", "--config", "/app/gunicorn.config.py"]
