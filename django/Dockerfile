FROM python:3.12.6-slim

ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONFAULTHANDLER 1
ENV PIPENV_VENV_IN_PROJECT 1

RUN pip install pipenv
RUN pip install django-cloudinary-storage

RUN useradd -ms /bin/bash my-user

USER my-user
WORKDIR /home/my-user/app

CMD ["tail", "-f", "/dev/null"]







# FROM python:3.12.6-slim

# ENV PYTHONDONTWRITEBYTECODE 1 # Prevents Python from writing pyc files to disc
# ENV PYTHONFAULTHANDLER 1 # Makes Python more verbose in case of an error
# ENV PIPENV_VENV_IN_PROJECT 1

# RUN pip install pipenv
# RUN pip install django-cloudinary-storage


# RUN useradd -ms /bin/bash my-user

# USER my-user

# WORKDIR /home/my-user/app
# CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]


# CMD tail -f /dev/null
