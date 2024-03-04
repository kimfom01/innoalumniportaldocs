# Backend

## Using Python

Create a virtual environment

```sh
python -m venv .env
```

Activate the environment

```sh
source .env/bin/activate
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
