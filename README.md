# Node.js Cloudant Sample

This application demonstrates how to use the Bluemix Cloudant NoSQL DB service.  It helps users organize their favorite files. The UI talks to a RESTful Express CRUD backend API.

[![Deploy to Bluemix](https://bluemix.net/deploy/button.png)](https://bluemix.net/deploy?repository=https://github.com/IBM-Bluemix/nodejs-cloudant)

## Run the app locally

1. [Install Node.js][]
+ cd into this project's root directory
+ Copy the value for the VCAP_SERVICES envirionment variable from the application running in Bluemix and paste it in a `vcap-local.json` file
+ Run `npm install` to install the app's dependencies
+ Run `npm start` to start the app
+ Access the running app in a browser at <http://localhost:3000>

[Install Node.js]: https://nodejs.org/en/download/


# Requesting to check a token : 

(1) POST Request to /checktoken 
(2) Add type & token as body parameters. Type is for the authentication provider.
    ex : 
    token : ds23e234fqwsfwef
    type : facebook
(3) Parse the response for error (if exists)
