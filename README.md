# My experience portofolio (pome as Proof Of My Experiences) Overview

## Overview

This is the central document for the design and implmentation of my experience portofolio (pome as Proof Of My Experiences) as a software programmer.

Below link navigates you to the page I have implemented.
http://pomefront.s3-website-ap-northeast-1.amazonaws.com/
![Page](./img/PomeFront.png)

### Development and Deployment Architecture

Folowing is the diagram showing the overview of the pipeline and infrastructure.
![Deploy](./img/deploy.png)

Implemented with
- Angular CLI: 14.2.6, Node: 16.18.0, Package Manager: npm 8.19.2 for the front end
- express.js: 4.17.1,  Node: 16.18.0, Package Manager: npm 8.19.2 for the front end for the backend API
- PostgreSQL 13.7 on AWS RDS for the backend DB
- [CircleCI](https://circleci.com/) for the CI/CD

For the detailed design and implemetation, please navigate to the links below.

## Front Web Application

### Software Design

https://github.com/HajimeK/pome_front/blob/main/architecture/overview.md


### package.json

https://github.com/HajimeK/pome_front/blob/main/package.json

|command|description|
|-|-|
|*npm install*| Install the dependent packages |
|*npm run build*| Build the applications to generate a distributable packages under dist folder|
|*npm run start*| Start the middleware |
### CI/CD with CircleCI

https://github.com/HajimeK/pome_front/blob/main/.circleci/config.yml

![CircleCI Frontend Deployment](./img/circleci_pome_front.png)
## Middleware API service

### Software Design

https://github.com/HajimeK/pome_api/blob/main/architecture/overview.md

|command|description|
|-|-|
|*npm install*| Install the dependent packages |
|*npm run build*| Build the applications to generate a distributable packages under dist folder|
|*npm run jasmine*| Automate the test |
|*npm run start*| Start the middleware |

### package.json

https://github.com/HajimeK/pome_api/blob/main/package.json

### CI/CD with CircleCI

https://github.com/HajimeK/pome_api/blob/main/.circleci/config.yml

![CircleCI Deployment](./img/circleci_pome_api.png)
## Database Tables Design

https://github.com/HajimeK/pome_db/blob/main/architecture/overview.md
