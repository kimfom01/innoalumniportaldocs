# Backend

> > This should work in an ideal world but the project structure and documentation of the project's repo is broken 😥 as such I just provided the typical setup for python backends

## Using Python

Create a virtual environment

```sh
python -m venv .env
```

Activate the environment

```sh
source .env/bin/activate
```

Create env file

```sh
touch .env
```

Fill the .env file with these config (replace with your appropriate config)

```plaintext
DATABASE_HOST=<127.0.0.1>
DATABASE_PORT=<5432>
DATABASE_PASSWORD=<password>
DATABASE_NAME=<inno_schedule>
DATABASE_USERNAME=<postgres>
SECRET_KEY=<3ebe2c9ec8f9a17da918>
ALGORITHM=<HS256>
ACCESS_TOKEN_EXPIRE_MINUTES=<30>
MAIL_USERNAME=<your mail (e.g. gmail)>
MAIL_PASSWORD=<password from mail>
MAIL_FROM=<your mail>
MAIL_PORT=<mail tls (e.g. 587 for gmail)>
MAIL_SERVER=<smtp.gmail.com for gmail>
MAIL_FROM_NAME=<your mail name>
```

Install the needed python packages

```sh
pip install -r requirements.txt
```

Run the python script:

```sh
python3 main.py
```

## Using docker

The port in docker is 8000 by default and locally you can map it to anything as you like

```sh
docker build -t alumni-backend
docker run -p 8000:8000 -d alumni-backend
```
