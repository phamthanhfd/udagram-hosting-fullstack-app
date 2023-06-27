# Hosting a Full-Stack Application

The project application, Udagram - an Image Filtering application, allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering service. It has two components:

- Frontend - Angular web application built with Ionic framework
- Backend RESTful API - Node-Typescript application

### Dependencies

```
- Node 16.15.0 (LTS) or more recent. While older versions can work it is advisable to keep node to latest LTS version
- npm 6.14.8 (LTS) or more recent, Yarn can work but was not tested for this project
- AWS CLI v2, v1 can work but was not tested for this project
- AWS EB CLI
- A RDS database running Postgres.
- A S3 bucket for FrontEnd.
- A Elastic Beanstalk for Backend


### Setup project

+ Clone project form: https://github.com/phamthanhfd/udagram-hosting-fullstack-app.git

+ Run the following command to install dependencies: `npm run frontend:install`

+ Run the following command to start: `npm run frontend:start`

+ Setup environment variables in .env file in udagram-api folder with your values
```

- POSTGRES_USERNAME = <Database_Username>
- POSTGRES_PASSWORD = <Database_Password>
- POSTGRES_DB = <Database_Name>
- POSTGRES_HOST = <Database_Host>
- AWS_REGION = us-east-1
- AWS_PROFILE = <AWS_Profile>
- AWS_BUCKET = <Bucket_Name>
- JWT_SECRET = <Jwt_Secret>

```

+ Run the following command to install dependencies: `npm run api:install`

+ Run the following command to start: `npm run api:start`

### Testing

- Run the following command to execute tests: `npm run frontend:test`

### AWS Setup
```

- S3: sherwinfd-thanhpv29.s3-website-us-east-1.amazonaws.com
- Elastic Beanstalk: sherwin-udagram-api.eba-6fdazw3d.us-east-1.elasticbeanstalk.com
- DB host RDS: database-1.clsp2eet6nij.us-east-1.rds.amazonaws.com
- DB port: 5432
- DB name: postgres

```

### CircleCI Pipelines

1. Build
    - Setup environment variables
    - Install NodeJS
    - Checkout code
    - Install FrontEnd dependencies
    - Install Backend dependencies
    - Build Frontend
    - Build Backend
2. Deploy
    - Setup environment variables
    - Install NodeJS
    - Setup Elastic Beanstalk CLI
    - Install AWS CLI
    - Configue AWS Access Key
    - Checkout code
    - Deploy
```
