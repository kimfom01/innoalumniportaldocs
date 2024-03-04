# Installation

## Alumni Portal Backend

### How to run

#### Using Python

- Open a shell/command line in this folder (better if it was after activating a python virtual env)
- Install the needed python packages

```bash
    pip install -r requirements.txt
```

- Run the python script:

```bash
    python3 main.py
```

#### Using docker

1. Here the image tag name is `alumni-backend` you can name it as you like
2. Also the port in docker is 8000 by default and locally you can map it to anything as you like

```bash
docker build -t alumni-backend
docker run -p 8000:8000 -d alumni-backend
```

## Inno-alumni-portal frontend

### How to run on local

- Open a shell/command line in this folder
- To `install` all packages (local to the repo) using `npm`

```bash
npm install
```

- To `build` the project for production

```bash
npm run build
```

- To `start` the project on development

```bash
npm start
```
