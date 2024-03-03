FROM python:latest

WORKDIR /app

EXPOSE 5050

COPY Pipfile Pipfile.lock ./

RUN pip install pipenv
RUN pipenv lock install --requirements > requirements.txt
RUN pip install requirements.txt


COPY . ./

CMD [ "python","main.py" ]