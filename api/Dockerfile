FROM python:latest

WORKDIR /app

EXPOSE 5050

COPY Pipfile Pipfile.lock ./

RUN pip install pipenv
RUN pipenv lock
RUN pipenv install --system --deploy



COPY . ./

CMD [ "python","main.py" ]