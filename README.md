# BeerBelly - A simple usage of Progressive Web App

[![Build Status](https://travis-ci.org/PolymerElements/polymer-starter-kit.svg?branch=master)](https://travis-ci.org/PolymerElements/polymer-starter-kit)

It is a simple Progressive Web App using polymer 2.0, Elasticseach and Firebase to social login

###
[Live demo](https://beerbelly-7202a.firebaseapp.com)

### Setup

##### Prerequisites


First, install [Polymer CLI](https://github.com/Polymer/polymer-cli) and [Firebase](firebase.google.com) using
[npm](https://www.npmjs.com) (we assume you have pre-installed [node.js](https://nodejs.org)).

    npm install -g polymer-cli
    npm install -g firebase

##### Install dependencies

    npm install
    bower install

### Start the development server

This command serves the app at `http://localhost:5000`
    firebase serve

### Build

This command performs HTML, CSS, and JS minification on the application
dependencies, and generates a service-worker.js file with code to pre-cache the
dependencies based on the entrypoint and fragments specified in `polymer.json`.
The minified files are output to the `build/unbundled` folder, and are suitable
for serving from a HTTP/2+Push compatible server.

In addition the command also creates a fallback `build/bundled` folder,
generated using fragment bundling, suitable for serving from non
H2/push-compatible servers or to clients that do not support H2/Push.

    polymer build


### Run tests

This command will run [Web Component Tester](https://github.com/Polymer/web-component-tester)
against the browsers currently installed on your machine:

    polymer test

