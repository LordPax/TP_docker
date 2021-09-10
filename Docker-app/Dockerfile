FROM python:3.7-alpine
LABEL maintainer="teddy gauthier"

WORKDIR /app
COPY requirements.txt .
RUN pip install -r requirements.txt

COPY app.py .
COPY config.py .

RUN adduser -D my-user -u 1000
USER 1000

ENTRYPOINT ["gunicorn"]
CMD ["--config", "config.py", "app:app"]
