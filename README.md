# Travis and SonarQube integration

This project was created just to know how [Travis](https://travis-ci.com/) and [SonarQube](https://www.sonarqube.org/) works.

### Travis Status

[![Build Status](https://travis-ci.com/guisfco/integration-test.svg?token=Ny7Ax4Uiscnhe6zwhRxz&branch=master)](https://travis-ci.com/guisfco/integration-test)

### SonarCloud Status

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=br.com.guisfco.test%3Atesting&metric=alert_status)](https://sonarcloud.io/dashboard?id=br.com.guisfco.test%3Atesting)

## Tutorial

#### In folder project

- Create a file ``.travis.yml`` into the project directory and paste the content from this repository.
- Create a file ``sonar-project.properties`` into the project directory and paste the content from this repository.

#### Now on https://travis-ci.com/

- Go to your repository and follow the steps: ``More options > Settings``
- On **Environment Variables** create a variable called ``SONAR_TOKEN`` and paste the project token that you received when you created the project on SonarQube
