FROM python:3

RUN apt-get update && \
    apt-get install -y python3-pip python-dev-is-python3 

WORKDIR /app

RUN pip3 install Flask requests Flask-MySQLdb==0.2.0

COPY . .

EXPOSE 5000

CMD ["python", "./app.py"]