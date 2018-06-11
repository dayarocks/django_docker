FROM python:3.6

WORKDIR /app
COPY django_docker django_docker

COPY manage.py /app/

COPY requirements.txt requirements.txt 
RUN pip install -r requirements.txt

EXPOSE 8000

ENTRYPOINT ["python", "manage.py", "runserver", "0.0.0.0:8000"]

