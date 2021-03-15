FROM python:3.6.0-alpine
FROM python:2.7
WORKDIR /app
RUN pip install --upgrade pip
ADD requirements.txt /app
RUN pip install -r requirements.txt
ADD . /app
ENV POST_DATABASE_HOST post_db
ENV POST_DATABASE posts
ENTRYPOINT ["python", "post_app.py"]

