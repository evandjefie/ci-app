# CI App

A basic continue integration project that build, test and push app to dockerhub.


## Prerequisites

- Dockerhub account created [Dockerhub](https://hub.docker.com/)
- Docker-compose installed [docker](https://docs.docker.com/compose/install/)
- Docker desktop (MAC or WINDOW) [docker](https://docs.docker.com/get-docker/)


## Installation

Clone project

```bash
  git clone https://github.com/evandjefie/ci-app.git
  cd ci-app
```

Launch jenkins server

```bash
  docker-compose up -d
```


Get secret from logs to Login to jenkins server

```bash
  docker-compose logs
```

Command output

```bash
ci-jenkins  | Jenkins initial setup is required. An admin user has been created and a password generated.
ci-jenkins  | Please use the following password to proceed to installation:
ci-jenkins  | 
ci-jenkins  | secret_locate_here
ci-jenkins  | 
ci-jenkins  | This may also be found at: /var/jenkins_home/secrets/initialAdminPassword
ci-jenkins  | 
ci-jenkins  | *************************************************************

```

Connect to http://localhost:8081

## Setup

- Create DockerHub Credential

  - Go to Dashboard>Administer Jenkins>Identifiers>System>Global identifiers (unlimited)
  - or http://localhost:8081/manage/credentials/

- Create Job

- Copy Jenkinsfile 
  - in your app repository
  - or in your created job

- Change value of environnement variables


## 🔗 Follow me
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://evandjefie.my.canva.site)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/evan-djefie)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/EvanDjefie)