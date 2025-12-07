FROM python:3.11-slim

WORKDIR /app

RUN apt update && apt upgrade -y 
COPY requirements.txt ./backend
RUN apt upgrade 
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

EXPOSE 5000

CMD ["python", "app.py"]
