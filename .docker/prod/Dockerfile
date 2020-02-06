FROM python:3.7
RUN pip install --upgrade pip
WORKDIR /app
COPY . .
RUN pip install -r requirements.txt
CMD [ "gunicorn", "-b", "0.0.0.0:8080", "app:app" ]
