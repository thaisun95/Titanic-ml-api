# docker/Dockerfile
FROM python:3.10-slim

WORKDIR /app

COPY ./app ./app
COPY ./model ./model
COPY ./requirements.txt .

RUN pip install --no-cache-dir -r requirements.txt

EXPOSE 80

## CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "8181"]

CMD ["uvicorn", "app.main:app", "--host", "0.0.0.0", "--port", "80"]
