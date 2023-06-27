# CircleCI Pipelines

When push code to `master` branch, the build will be triggered

```
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
