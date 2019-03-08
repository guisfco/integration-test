# Travis and SonarQube Integration

This project was created just to know how [Travis](https://travis-ci.com/) and [SonarQube](https://www.sonarqube.org/) integration works.

### Travis Status

[![Build Status](https://travis-ci.com/guisfco/integration-test.svg?token=Ny7Ax4Uiscnhe6zwhRxz&branch=master)](https://travis-ci.com/guisfco/integration-test)

### SonarCloud Status

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=br.com.guisfco.test%3Atesting&metric=alert_status)](https://sonarcloud.io/dashboard?id=br.com.guisfco.test%3Atesting)

## Tutorial

### First steps

First of all you will need to import your repository to [Travis](https://travis-ci.com/) and later on analyze the project on [SonarCloud](https://sonarcloud.io/).

Pay attention to the SonarCloud configuration, because you will receive a token when you are creating the project. Also you will have to run some commands on Maven. If you're using **Intellij** you can run it with _Execute Maven Goal_, just paste it and follow the next steps.

#### In folder project

- Create a file ``.travis.yml`` into the project directory and paste the content from this repository.
- Create a file ``sonar-project.properties`` into the project directory and paste the content from this repository.

#### Now on https://travis-ci.com/

- Go to your repository and follow the steps: ``More options > Settings``.
- On **Environment Variables** create a variable called ``SONAR_TOKEN`` and paste the analyzed project token that you received when you created the project on SonarCloud.

#### Moving to ``.travis.yml`` file

- Replace the value of ``organization:`` with your organization _(Organization Key found at SonarCloud)_.
- The ``install`` and ``script`` sections are configured to a **_Maven Project_**, so if you're not using it you'll probably need another commands.

#### Ending at ``sonar-project.properties`` file

- Replace the value of ``sonar.projectKey:`` with your project key _(Probably will be next to Organization Key on SonarCloud)_.



![Done](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTyTYCiB7LcZprNB_T2FG_fcKEHRp_bckXBCWjv88vopIHG1KrE)
