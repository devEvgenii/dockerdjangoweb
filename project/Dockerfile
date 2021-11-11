FROM python:2
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1
RUN mkdir -p /code
WORKDIR /code
COPY requirements.txt /code/
RUN pip install -r requirements.txt
COPY . /code
EXPOSE 80
CMD [ "python", "./manage.py", "runserver", "0.0.0.0:80" ]
