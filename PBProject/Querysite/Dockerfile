FROM python:3

ENV PYTHONUNBUFFERED 1
RUN mkdir /app
WORKDIR /app
COPY requirements.txt /app/
RUN pip install -r requirements.txt
RUN pip install requests
COPY . /app/
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]