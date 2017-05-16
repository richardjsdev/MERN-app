# MERN stack starter

[![Build Status](https://travis-ci.org/rfdickerson/mern-example.svg?branch=master)](https://travis-ci.org/rfdickerson/mern-example)

## Getting Started

1. Install dependencies with 

  ```
  npm install
  ```
  
  or 
  
  ```
  yarn
  ````

2. Install MongoDB
  
3. Start the development environment

  ```
  npm run start-dev
  ```
  
  or 
  
  ```
  yarn start-dev
  ```

## Docker Compose

If you use Docker and Docker Compose, you can start the entire project with:

```
docker-compose up
```
 
## Configuration (Optional)

You can create a `.env` file for specifying credential information for MongoDB. 

Create a new file called `.env` and put YAML:

```yaml
MONGO_URL=mongodb://localhost:27017/comments
MONGO_USER=username
MONGO_PASSWORD=password
```

or instead, you can use the equivalent JSON:

```json
{
  "mongo": {
    "url": "mongodb://localhost:27017/comments",
    "user": "username",
    "password": "password"
  }
}
```

Where the URL, username, and password are set to your preferences.

## Docker Development run

You can set up a local Docker development environment by building the image:

```
docker build -f Dockerfile-tools -t rfdickerson/mern-example .
```

And running the image:

```
docker run -p 3000:3000 -v ${PWD}:/app -t rfdickerson/mern-example
```

## Libraries

  - [axios](https://github.com/mzabriskie/axios) - promise-based HTTP client
  - [foreman](https://github.com/strongloop/node-foreman) - a Procfile-based application utility
  - [mongoose](http://mongoosejs.com/) - mongodb object modelling
  - [express](https://expressjs.com/) - minimalist Node.js framework
  - [react](https://facebook.github.io/react/) - JS library for building user interfaces
