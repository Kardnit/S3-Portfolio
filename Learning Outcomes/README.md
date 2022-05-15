# Welcome to my Learning Outcomes!

## Table of Contents

1. [Web Application](#Web-Application)
2. [Software Quality](#Software-Quality)
3. [Agile Method](#Agile-Method)
4. [CI/CD](#CI/CD)
5. [Cultural Differences and Ethics](#Cultural-Differences-and-Ethics)
6. [Requirements and Design](#Requirements-and-Design)
7. [Business Processes](#Business-Processes)
8. [Professional](#Professional)

## 1) Web Application

### Mi-Madre Front-end

Repository: [MiMadre](https://github.com/Kardnit/Mi-Madre)

#### Single page
In the application we can call the API services as seen in the picture below.

![Frontend](https://user-images.githubusercontent.com/73908937/168483667-16112fb9-5262-4b53-bb5f-77ca95b6faaa.png)


#### Auth0
...


### Mi-Madre Services

Repository: [Mi-Madre Services](https://github.com/Kardnit/Mi-Madre-Backend)

Mi-Madre Services provides all the materials that are needed in the website.

![Backend](https://user-images.githubusercontent.com/73908937/168484415-8be31d37-2d06-4818-8f93-3ed9438accdd.png)

![Workbench](https://user-images.githubusercontent.com/73908937/168484789-44843e33-83bb-4050-a2a2-0262c8aa6c10.png)


Link: [Services](mi-madre-7ps3n.ondigitalocean.app)

For the services I use Restless API because the database requires username and password for security reasons so instead of using something like SwaggerUI thats accessible from outside I used MySQL Workbench if I needed to do some alterations as seen in the picture above but eveything is accessible from the website so there is no point using MySQL Workbench anymore.

## 2) Software Quality

### 1. DigitalOcean Database

I use DigitalOcean Database to display the products that my clients wishes to and testing purposes (by creating testing tables) the reason I use this database is 

1) Easy setup and maintenance
2) Highly scalable
3) Daily backups
4) Automated failover
5) Fast and reliable performance
6) End-to-end security

```properties
spring.datasource.url=jdbc:mysql://username:password@dbaas-db-9653187-do-user-11378243-0.b.db.ondigitalocean.com:25060/mi-madre?ssl-mode=REQUIRED
spring.mvc.throw-exception-if-no-handler-found=true
spring.resources.add-mappings=false
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jackson.serialization.fail-on-empty-beans=false
```

### 2. Unit Testing

...

### 3. Integration Testing

...

### 4. Automated testing

...

### 5. SonarCloud

I use SonarCloud to check the quality of the code whenever I push something new to my repository and see if there are any problems in it.

![SonarCloud](https://user-images.githubusercontent.com/73908937/168485474-5213f916-9e1d-4064-b654-3b98aa30d65d.png)

## 4)Agile Method

In this semester I Implemented the usage of SCRUM along with the usage of the project board on JIRA and Shortcut. I had multiple cycles of development (sprints) with 1 cycle containing 2-3 weeks. In my group we had daily meetings in the morning and also did peer-feedback occasionally, to clear up any problems if needed.

![Jira](https://user-images.githubusercontent.com/73908937/168486773-d7e882a8-2fac-4977-83bd-f3f1b21bb43e.png)

![Shortcut](https://user-images.githubusercontent.com/73908937/168486784-36156e7c-abed-4134-af07-6c802d82839e.png)


## 4)CI/CD
Below you can see my first workflow file that uses dockerhub to deploy my project so I can publish it from DigitalOcean

![Deploy Workflow](https://user-images.githubusercontent.com/73908937/168487682-cf3f5d45-cd24-4c8f-b375-69b6183a3283.png)


Below you can see my second workflow file that uses sonarcloud to check the quality of my code.

![SonarCloud Workflow](https://user-images.githubusercontent.com/73908937/168487641-af6006a7-7b9d-42c8-ac13-7017d1a7f75b.png)


### Docker Hub

In the picture below you can see that whenever we push a project it first builds it and after that deploys it.

![Docker Hub](https://user-images.githubusercontent.com/73908937/168486465-07482338-86b0-4842-b922-6c63403e6bff.png)
