# Hosting a Full-Stack Application

## Overview

In this project we will use CircleCi to create pipeline that will build and deploy front and backend of our application using AWS services.

### AWS Services Used

- RDS for the database
![RDS](./screenshots/rds.png)

- ElasticBeanstalk for the (backend) API deployment
![ElasticBeanstalk](./screenshots/eb.png)

- S3 for (frontend) web hosting
![S3](./screenshots/s3.png)

### Circleci

- We used circleci for ci/cd proccess
![S3](./screenshots/circleci_overview.png)
![S3](./screenshots/circleci_build.png)
![S3](./screenshots/circleci_deploy.png)

- CircleCi secrets
![Secrets](./screenshots/secrts.png)

[APP URL](http://udagram-udacity.s3-website-us-east-1.amazonaws.com/)

![WORKING APP](./screenshots/working_app.png)

### Dependencies

```text
- Node v14.15.1 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version

- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project

- AWS CLI v2, v1 can work but was not tested for this project

- A RDS database running Postgres.

- A S3 bucket for hosting uploaded pictures.

```

### Installation

Provision the necessary AWS services needed for running the application:

1. In AWS, provision a publicly available RDS database running Postgres. <Place holder for link to classroom article>
1. In AWS, provision a s3 bucket for hosting the uploaded files. <Place holder for tlink to classroom article>
1. Export the ENV variables needed or use a package like [dotnev](https://www.npmjs.com/package/dotenv)/.
1. From the root of the repo, navigate udagram-api folder `cd starter/udagram-api` to install the node_modules `npm install`. After installation is done start the api in dev mode with `npm run dev`.
1. Without closing the terminal in step 1, navigate to the udagram-frontend `cd starter/udagram-frontend` to intall the node_modules `npm install`. After installation is done start the api in dev mode with `npm run start`.

## Testing

This project contains two different test suite: unit tests and End-To-End tests(e2e). Follow these steps to run the tests.

1. `cd starter/udagram-frontend`
1. `npm run test`
1. `npm run e2e`

There are no Unit test on the back-end

### Unit Tests

Unit tests are using the Jasmine Framework.

### End to End Tests

The e2e tests are using Protractor and Jasmine.

## Built With

- [Angular](https://angular.io/) - Single Page Application Framework
- [Node](https://nodejs.org) - Javascript Runtime
- [Express](https://expressjs.com/) - Javascript API Framework

## License

[License](LICENSE.txt)
