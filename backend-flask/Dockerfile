FROM python:3.10-slim-buster


# Set the working directory in the container
WORKDIR /backend-flask

COPY requirements.txt requirements.txt

RUN pip3 install -r requirements.txt


COPY . .

ENV FLASk_ENV=development


# Command to run on container start
EXPOSE ${PORT}
# python3 -m flask run --host=0.0.0.0 --port=4567
CMD [ "python3", "-m",  "flask", "run", "--host=0.0.0.0", "--port=4567" ]