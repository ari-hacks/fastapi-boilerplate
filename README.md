# FastApi Skeleton
A Boilerplate FastApi project

![MIT license](https://img.shields.io/badge/License-MIT-blue.svg) [![Build Status](https://api.travis-ci.com/ari-hacks/fastapi-skeleton.svg?branch=master)](https://travis-ci.com/ari-hacks/fastapi-skeleton)


## Features 
- [x] Boilerplate project structure  
- [x] Asynchronous API 
- [ ] User login and Authentication 
- [ ] Postgres DB storage? Redis? 
- [x] Travis CI configuration before deploy 
- [x] API testing with `pytest` 
- [x] Pipenv dependency management 
- [ ] Docker containerization and deploy to Heroku   

## Set up

### Requirements

- [Python](https://www.python.org/) 3.8.1

## Running Locally 

1. Clone this repository and `cd` into it

    ```bash
        → git clone https://github.com/ari-hacks/fastapi-skeleton.git
        → cd fastapi-skeleton
    ```
2. Pipenv dependency management 

    ```bash
        #add pipenv with python 3
        → pipenv --three
    ```
    ```bash
        #run pipenv 
        → pipenv shell
    ```
    ```bash
        #install dependencies  
        → pipenv install fastapi
        → pipenv install uvicorn
    ```
    ```bash
        #add requirements.txt   
        → pip3 freeze > requirements.txt
    ```
3. [Install & Run in docker](https://hub.docker.com/) 
4. Build Docker Image 
    ```bash
        ➜ docker build -t app .
    ```
5. Start Docker container 
    ```bash
        ➜ docker run -d --name fastapi-skeleton-container -p 80:80 app
    ```
6. Run the application
   ```bash 
    Uvicorn running on http://0.0.0.0:80/users/health-check 
   ```
7. Deploy to Heroku 

```bash
uvicorn app.main:app --reload 

#uvicorn runs on http://127.0.0.1:8000    
```

## Deploy pre-configured (Docker Deploy)

