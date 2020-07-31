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

If you prefer to compile our project in Polymer you must compile it with the next command:

    polymer build

And you can use the Polymer wrapped with NodeJS just following the next command:

    npm start

Note: This configuration you can see in the file server.js

And finally this project execute on serves the app at 'http://localhost:3000/'.
