FROM django

RUN apt update
RUN django-admin startproject mysite
WORKDIR ./mysite
RUN python manage.py startapp polls

ADD ./polls/* ./polls/*
ADD ./mysites ./mysite/

EXPOSE 8000
STOPSIGNAL SIGINT
ENTRYPOINT ["python", "manage.py","runserver", "0.0.0.0:8000"]

EXPOSE 8000