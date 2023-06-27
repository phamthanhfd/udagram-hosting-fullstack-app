# Hosting a Full-Stack Application

The project application, Udagram - an Image Filtering application, allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering service. It has two components:

- Frontend - Angular web application built with Ionic framework
- Backend RESTful API - Node-Typescript application

> This is an simple description, you should read the documents about Infrastructure and Pipelines in the readme folder.

### Dependencies

```
- Node 16.15.0 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version
- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project
- AWS CLI
- AWS EB CLI
- A RDS database running Postgres.
- A S3 bucket for FrontEnd.
- A Elastic Beanstalk for Backend
```

### Setup project

1. Clone project form: https://github.com/phamthanhfd/udagram-hosting-fullstack-app.git

2. Run the following command to install dependencies: `npm run frontend:install`

3. Run the following command to start: `npm run frontend:start`

4. Setup environment variables in .env file in udagram-api folder with your values

5. Run the following command to install dependencies: `npm run api:install`

6. Run the following command to start: `npm run api:start`

### Testing

- Run the following command to execute tests: `npm run frontend:test`
