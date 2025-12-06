FROM python:3.11-slim

WORKDIR /app

COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .

# Variables d'environnement par défaut
ENV DB_HOST=db
ENV DB_NAME=logs_db
ENV DB_USER=logs_user
ENV DB_PASSWORD=logs_password
ENV DB_PORT=5432

EXPOSE 5000

CMD ["python", "app.py"]
