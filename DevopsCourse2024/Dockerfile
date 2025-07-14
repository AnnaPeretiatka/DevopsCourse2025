FROM python:latest

WORKDIR /app

ENV FLASK_APP=flaskr
ENV FLASK_ENV=development

COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt

COPY . .

RUN flask init-db

EXPOSE 5000

CMD ["flask", "run", "--host=0.0.0.0"]
~

