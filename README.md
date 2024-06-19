# Question 3: API Creation

## Problem Statement:
Create a simple RESTful API using Flask. The API should have one endpoint /greet that accepts a GET request and returns a JSON response with a greeting message.

### Requirements:


* Use the Flask or Fastapi library.
* The endpoint /greet should accept a query parameter name and return a JSON response in the format: {"message": "Hello,
{name}!"} .
* If the name parameter is not provided, the response should be {"message": "Hello, World!"} .


## Run
```
docker compose up --build -d
```
and run below to test api with query param
```
curl "http://localhost:5000/greet?name=John"
```
and run below to test api without query param
```
curl "http://localhost:5000/greet"
```
and run below for cleanout
```
docker-compose down --rmi all
```

## Demo
![demo](https://github.com/thomas-chiang/api_creation/assets/84237929/0aa22e6d-ac81-4a3f-a485-341079e8b9db)

