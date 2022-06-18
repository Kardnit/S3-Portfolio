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
I decided to make Mi-Madre using React since it is one of the most powerful and popular frameworks/libraries. React being so popular helps me find and learn new features. Also, Mi-Madre is a single-page app due to its advantages, such as having a better user experience, performance, reusability, and optimization. Normally React apps use JavaScript, and this causes difficulty in tracing errors, therefore I decided to use TypeScript.

![Frontend](https://user-images.githubusercontent.com/73908937/168483667-16112fb9-5262-4b53-bb5f-77ca95b6faaa.png)

### Fullstack
Mi-Madre Services used Spring Framework (a robust programming and configuration model) to simplify the app's development on the popular Java EE technology stack from Oracle, which was very complex and difficult to use at the time.

![Backend](https://user-images.githubusercontent.com/73908937/168484415-8be31d37-2d06-4818-8f93-3ed9438accdd.png)

Link (it will give a Whitelabel error because you need to add /work, /patterndesign, or /product to the link): ![Services](mi-madre-7ps3n.ondigitalocean.app)

I used Restful API for the services as the user has no contact with the back-end, so there is no need for a GUI. 

The website has Object Relational Mapping and Asynchronous Communication.

## 2) Software Quality

### 1. JWT
I used JWT since JSON is neater than its competitors, so in an encoded form, it is smaller in size, and this also makes it good to pass in environments like HTML or HTTP. It has less chance of producing security holes. Since it is easier to work with than SAML, it is more common. Furthermore, it is easier to process on user devices, considering it is used on an internet scale.

JWT Research: [JWT Research](https://github.com/Kardnit/Portfolio/tree/main/Researchs)

### 2. Auth0
I used Auth0 as it is a SaaS-based identity management platform with features, such as single sign-on, social media logins, and secure identity storing, with industry-standard protocols. It is one of the best identity management products on the market.

![Auth0](https://user-images.githubusercontent.com/73908937/172950036-4590240a-0b2a-4cab-bea6-700fa857ec44.png)

### 3. Testing
For now, I only used Unit Testing and Integration Testing in this project as the project is not only for this semester, but a web application that will be used on a real business, so there will be many changes in the future of this project and doing testing these changes will be time and money consuming for the client. I used Unit Testing since it ensures that multiple aspects of the endpoint properly work within the scope of the endpoint itself, on a local level, and I used Integration Testing to make sure multiple endpoints work/interact with one another correctly.

![Unit Testing](https://user-images.githubusercontent.com/73908937/172950676-f56d2363-225d-48a2-b1a4-b5e98ed010fb.png)

![Integration Testing](https://user-images.githubusercontent.com/73908937/172978410-9d76f81f-67ca-4637-adf5-592876c2e36e.png)

Testing Research: [Testing Research](https://github.com/Kardnit/Portfolio/tree/main/Researchs)

### 4. DigitalOcean Database
I used DigitalOcean Database to store/display the products my clients requested and for testing purposes (by creating testing tables). My reasons for using this database are as follows:

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
![Workbench](https://user-images.githubusercontent.com/73908937/168484789-44843e33-83bb-4050-a2a2-0262c8aa6c10.png)

### 5. Static/Dynamic code analysis

|App/Tool|Type|example| 
|---:|---|---| 
| **SonarCloud**| Static | I used SonarCloud to check the quality of the code whenever I pushed something new to my repository and see if there were any problems in it so that I could fix them without any delay and have the most optimal coding. |
| **Postman** | Dynamic | I used Postman for time-effective troubleshooting and analysis when dealing with HTTP/HTTPS requests and responses.

![SonarCloud](https://user-images.githubusercontent.com/73908937/168485474-5213f916-9e1d-4064-b654-3b98aa30d65d.png)

![Postman](https://user-images.githubusercontent.com/73908937/172945893-707b647e-f677-42ca-8c7e-e1036d42b185.png)

## 4)CI/CD

1) Continuous Integration
DigitalOcean, combined with Github actions, is a powerful tool for effective continuous integration workflows. It allows me to work on the code and do automatic testing after each git push and, once tests have passed successfully, I can move further down into the CD pipeline. This improves the reliability of the software.

2) Continuous Deployment
Following the CI workflow, continuous deployment consists of bringing new source code to DigitalOcean repositories and pushing the changes into production in an automated way. This allows me to save time and mitigates problems that could occur when trying to deploy non-functioning code into production and only figuring out the errors later on.

Below you can see my first workflow file that uses docker hub to deploy my project so I can publish it from DigitalOcean.
![Deploy Workflow](https://user-images.githubusercontent.com/73908937/168487682-cf3f5d45-cd24-4c8f-b375-69b6183a3283.png)

Below you can see my second workflow file that uses SonarCloud to check the quality of my code.
![SonarCloud Workflow](https://user-images.githubusercontent.com/73908937/168487641-af6006a7-7b9d-42c8-ac13-7017d1a7f75b.png)

Below you can see that whenever I push a project, it first builds it and, after that, deploys it.
![Docker Hub](https://user-images.githubusercontent.com/73908937/168486465-07482338-86b0-4842-b922-6c63403e6bff.png)

Below you can see how I organize my time while developing using Jira.

![Jira](https://user-images.githubusercontent.com/73908937/174265213-be0adf17-da4a-462b-9da5-d7ef6bc5e31b.png)

## 8) Professional

This semester I have done two types of research (JWT and Testing). I have chosen these topics because I want to deliver a secure and error-free app to my client.

JWT Research: [JWT Research](https://github.com/Kardnit/Portfolio/tree/main/Researchs)

Testing Research: [Testing Research](https://github.com/Kardnit/Portfolio/tree/main/Researchs)

While doing these researches, I have used DOT framework research methods and implemented 5 of these that were under the Library, Field, and Showroom categories to make sure the research I have done was as accurate as possible, and these methods were

### 1. Available product analysis
### 2. Community research
### 3. Document analysis
### 4. Ethical check
### 5. Peer review

I thought I did well this semester by learning new technologies according to my requirements and implementing them in my project in the related part. I have learned more than seven, so it was a load of stuff in a limited amount of time. I want to improve doing research, using agile methods, and software testing for the following semesters. I have implemented all the things I wanted to improve, but I believe these topics are the ones I have room to improve most.