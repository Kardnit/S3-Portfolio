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
I use JWT because JSON is neater than its competitors so in an encoded form its smaller in size and this also makes it good to pass in environments like HTML or HTTP. It has less chance of producing security holes. Because its easier to work with than SAML its more common. Also, it’s easier to process on user’s devices considering it is used at internet scale.

JWT Research: ![JWT Research](https://github.com/Kardnit/Portfolio/tree/main/Research)

### 2. Auth0
I use Auth0 because it is a SaaS-based identity management platform that has features such as single sign-on, social media logins, secure identity storing, etc. with industry-standard protocols and it is one of the best identity management product on the market.

![Auth0](https://user-images.githubusercontent.com/73908937/172950036-4590240a-0b2a-4cab-bea6-700fa857ec44.png)

### 3. Testing
For now I only use Unit Testing and Integration Testing in this project because the project is not only for this semester but a web application that will be used on a real business so there will be many changes in the future of this project and doing testing for stuff that will change will be time and money consuming for the client. The reason I use Unit Testing is it ensures that multiple aspect of the endpoint work properly within the scope of the endpoint itself, on a local level and the reason I use Integration Testing is to make sure multiple endpoints work/interact with one another correctly.

![Unit Testing](https://user-images.githubusercontent.com/73908937/172950676-f56d2363-225d-48a2-b1a4-b5e98ed010fb.png)

![Integration Testing](https://user-images.githubusercontent.com/73908937/172978410-9d76f81f-67ca-4637-adf5-592876c2e36e.png)

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
| **Postman** | Dynamic | I use Postman because it allows to do time-effective troubleshooting and analysis when dealing with http/https requests and responses

![SonarCloud](https://user-images.githubusercontent.com/73908937/168485474-5213f916-9e1d-4064-b654-3b98aa30d65d.png)

![Postman](https://user-images.githubusercontent.com/73908937/172945893-707b647e-f677-42ca-8c7e-e1036d42b185.png)

## 4)CI/CD

1) Continuous Integration
DigitalOcean in combination with Github actions is a very powerful tool to perform effective continuous integration workflows. It allows me to work on code and do testing automatically after each git push and, once tests have passed successfully, can move further down into the CD pipeline. This improves reliability of the software.

2) Continuous Deployment
Following the CI workflow, continuous deployment consists of bring new source code to DigitalOcean repositories and subsequently pushing the changes into production in an automated way. This allows me to save time and mitigates problems that could occur if trying to deploy not functioning code into production and only figuring the errors later on.

Below you can see my first workflow file that uses dockerhub to deploy my project so I can publish it from DigitalOcean
![Deploy Workflow](https://user-images.githubusercontent.com/73908937/168487682-cf3f5d45-cd24-4c8f-b375-69b6183a3283.png)

Below you can see my second workflow file that uses SonarCloud to check the quality of my code.
![SonarCloud Workflow](https://user-images.githubusercontent.com/73908937/168487641-af6006a7-7b9d-42c8-ac13-7017d1a7f75b.png)

In the picture below you can see that whenever we push a project it first builds it and after that deploys it.
![Docker Hub](https://user-images.githubusercontent.com/73908937/168486465-07482338-86b0-4842-b922-6c63403e6bff.png)
