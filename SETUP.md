# Setup

## Pre-requisites
### Front-End:
To run the front-end is required to clone the repository.

    git clone https://github.com/kukulhan/ibmfrontend.git

Install [Polymer CLI](https://github.com/Polymer/polymer-cli) using
[npm](https://www.npmjs.com) (we assume you have pre-installed [node.js](https://nodejs.org)).

    npm install -g polymer-cli --unsafe-perm

Note: We use to Polymer version 2.0

    polymer --version

Initialize project from template

    npm install

### Start the development server

You need install all dependencies (we assume you have pre-installed [bower](https://bower.io/)).

    bower install

This command serves the app at `http://127.0.0.1:8081` and provides basic URL routing for the app:

    polymer serve

### Back-End:
To run the back-end is required to clone the repository.

    git clone https://github.com/kukulhan/imbbackend.git

We assume you have pre-installed [node.js](https://nodejs.org)) and [npm](https://www.npmjs.com)

Initialize project from template

    npm install

And finally this project execute on serves the app at `http://localhost:3000/`.

### Twitter:
You need create an account in **Twitter Developer Labs** for you can configure your own credentials an put this values in the environment variables (file .env)
For more information...[api twitter](https://developer.twitter.com/en)

### IBM Watson Assistant:
Also, you need create an account in **IBM Watson Assistant** and put your own credentials. For more information...[ibm watson](https://www.ibm.com/cloud/watson-assistant/)

### Database MongoDB:
You need create a database, in this project we made a cluster in **MongoDB Atlas Cloud**. For more information...[mongodb](https://www.mongodb.com/cloud/atlas)

### Create a container with Docker:
We separate front and back in different containers, so each architecture has the configuration for you can deploy own project in docker.
This configuration are in the file dockerfile. (We assume you have pre-installed [docker](https://docs.docker.com/engine/install/))

Therefore, you need compile our **Front-End** in Polymer with the next command:

    polymer build

This project was configured the Polymer wrapped with NodeJS just following the next command (This step it's not necessary):

    npm start

Note: This configuration you can see in the file server.js The project execute on serves the app at `http://localhost:3000/`.

Then build the project in docker:

    docker build -t iknelia/frontend .

We need change the project's port on serves the app at `http://localhost:3001/`.

    docker run -p 3001:3000 -d iknelia/frontend

And you need compile our **Back-End** in Docker with the next command:

    docker build -t iknelia/backend .

We don't need change the project's port on serves.

    docker run -p 3000:3000 -d iknelia/backend

You can verify the containers is executing with:

    docker ps

And that's all! :)
