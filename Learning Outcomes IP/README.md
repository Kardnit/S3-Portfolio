# Welcome to my Learning Outcomes!

## Table of Contents

1. Web Application
2. Software Quality
4. CI/CD
8. Professional

## Mi-Madre
Link: [MiMadre](https://mimadre-7ll8w.ondigitalocean.app/)

## Mi-Madre Front-end
Repository: [MiMadre Frontend](https://github.com/Kardnit/Mi-Madre)

## Mi-Madre Back-end
Repository: [MiMadre Backend](https://github.com/Kardnit/Mi-Madre-Backend)

## 1) Web Application

### User-friendly
I decided to make Mi-Madre using React because it is one of the most powerfull and popular framework/library.React being so popular helps me when I need to find/learn new stuff about it. Also Mi-Madre is a single-page app because of its advantages like having better user experience, performance, reusability and optimization. Normally single-page apps use JavaScript and this causes difficulty for tracing errors so I decided to use TypeScript.

![Frontend](https://user-images.githubusercontent.com/73908937/168483667-16112fb9-5262-4b53-bb5f-77ca95b6faaa.png)

### Fullstack
Mi-Madre Services use Spring Framework (a robust programming and configuration model) to simplify the development of the app on the popular Java EE technology stack from Oracle, which was very complex and difficult to use at the time.

![Backend](https://user-images.githubusercontent.com/73908937/168484415-8be31d37-2d06-4818-8f93-3ed9438accdd.png)

![Workbench](https://user-images.githubusercontent.com/73908937/168484789-44843e33-83bb-4050-a2a2-0262c8aa6c10.png)

Link (it will give a Whitelabel error because you need to add /work, /patterndesign or /product to the link): [Services](mi-madre-7ps3n.ondigitalocean.app)

For the services I use Restful API because the user has no contact with the back-end so there is no need for a gui. 

The website has Object Relational Mapping and Asynchronous Communication.

## 2) Software Quality

### 1. JWT
...

JWT Research: ![JWT Research](https://github.com/Kardnit/Portfolio/tree/main/Research)

### 2. Auth0
...

### 3. Unit Testing
...

### 4. DigitalOcean Database
I use DigitalOcean Database to store/display the products that my clients wishes to and testing purposes (by creating testing tables) the reasons I use this database are 

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
### 5. Static/Dynamic code analysis

|App/Tool|Type|example| 
|---:|---|---| 
| **SonarCloud**| Static | I use SonarCloud to check the quality of the code whenever I push something new to my repository and see if there are any problems in it so I can fix these problems without any delay and have the most optimal coding. |
| **Postman** | Dynamic | I use Postman

1) Static
I use SonarCloud to check the quality of the code whenever I push something new to my repository and see if there are any problems in it so I can fix these problems without any delay and have the most optimal coding.

![SonarCloud](https://user-images.githubusercontent.com/73908937/168485474-5213f916-9e1d-4064-b654-3b98aa30d65d.png)

2) Dynamic
I use Postman


## 4)CI/CD
Below you can see my first workflow file that uses dockerhub to deploy my project so I can publish it from DigitalOcean

![Deploy Workflow](https://user-images.githubusercontent.com/73908937/168487682-cf3f5d45-cd24-4c8f-b375-69b6183a3283.png)


Below you can see my second workflow file that uses sonarcloud to check the quality of my code.

![SonarCloud Workflow](https://user-images.githubusercontent.com/73908937/168487641-af6006a7-7b9d-42c8-ac13-7017d1a7f75b.png)


### Docker Hub
In the picture below you can see that whenever we push a project it first builds it and after that deploys it.

![Docker Hub](https://user-images.githubusercontent.com/73908937/168486465-07482338-86b0-4842-b922-6c63403e6bff.png)
