# POS – “Point of Sale” (FrontEnd)
-----------------------------------------------------------------

## 1. [Documentation](https://github.com/togetherGithub/Point-Of-Sale)

## 2. Automation Source Code
* 2.1 [Backend](https://github.com/togetherGithub/Point-Of-Sale/tree/main/rest-service)
* 2.1 [Frontend](https://github.com/togetherGithub/Point-Of-Sale/tree/main/web-client-v2)

## Prerequisites

### Install Node JS
Refer to https://nodejs.org/en/ to install nodejs

## Development server

Run `npm start` for a dev server. Navigate to `http://localhost:3000/`. The app will automatically reload if you change any of the source files.

Or

### How to start

**Note** that this seed project requires **node.

In order to start the project use:

```bash
# install the project's dependencies
$ npm install
# watches your files and uses livereload by default run `npm start` for a dev server. Navigate to `http://localhost:3000/`. The app will automatically reload if you change any of the source files.
$ npm start
# prod build, will output the production application in `dist`
# the produced code can be deployed (rsynced) to a remote server
$ npm run build
```

## Application design

#### Components

1. **Customers** Component : This Component displays a list of customers. This Component gets the data from a json file in assets folder

2. **CustomerDetails** Component : This Component Displays the details of the selected customer. This Component gets its data from a json file in assets folder as well. This Component is the Child Component of *Customers* Component

#### HTTP client

**axios** library is used to make HTTP Calls

## Resources

**create-react-app** : The following link has all the commands that can be used with create-react-app
https://github.com/facebook/create-react-app

**ReactJS** : Refer to https://reactjs.org/ to understand the concepts of ReactJS

**React Bootstrap** : Refer to https://react-bootstrap.github.io/getting-started/introduction/ to understand how to use React Bootstrap
