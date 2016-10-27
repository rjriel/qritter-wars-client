# qritter-wars-client

## Overview

This is a bare bones client for the Qritter Wars game.

## Getting started
To get up and running please follow the following steps

1. clone the repo `git clone https://github.com/rjriel/qritter-wars-client.git`

  **OR**

  download and unzip the package at [https://github.com/rjriel/qritter-wars-client/archive/master.zip](https://github.com/rjriel/qritter-wars-client/archive/master.zip)
  
2. run `npm install` to install dependencies
3. If you haven't already created a qritter, do so by posting to the API endpoint `http://<server>:<api port>/signup` with a json body like below:

  ```
  {
	"name": "<qritter name>"
  }
  ```
  
  The result will be a json object with the `apiId` and `apiSecret` in the body.
4. add a config.json file to the root of the project. It should look like the following:

  ```
  {
    "host": "<qritter wars server>",
    "socketPort": <qritter wars socket port>,
    "apiPort": <qritter wars REST API port>,
    "apiId": "<qritter API ID>",
    "apiSecret": "<qritter API Secret>"
  }
  ```
 
5. run `node index.js`
