# node.js
var express = require('express');
var path = require('path');
var cookieParser = require('cookie-parser');
var bodyParser = require('body-parser');
var app = express();
app.use(bodyParser.json());
app.use(bodyParser.urlencoded({ extended: false }));
app.use(cookieParser());
app.use(express.static(path.join(__dirname, 'public')));
module.exports = app;

{
  "name": "mongoose-app",
  "version": "0.0.0",
  "private": true,
  "scripts": {
    "start": "node ./app"
  },
  "dependencies": {
    "body-parser": "~1.15.1",
    "cookie-parser": "~1.4.3",

    "express": "~4.13.4"

  }
}
