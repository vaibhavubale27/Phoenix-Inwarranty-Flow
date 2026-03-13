# Postman API Automation Integration with Github Actions

This repository for demonstration for POC for Integrating tests with github Actions. The test are written in postman and they are executed on the VM with the help of newman and newman-reporter-html.extra.
Github actions will trigger the project executions on every push to the main branch.You can also execute project manually using workflow_dispatch.The project runs on schedule time with the help of cron job.

The html reports are archived and kept in the artifact section for the team to download it.Along with that they can view the report from the github page : https://vaibhavubale27.github.io/Phoenix-Inwarranty-Flow/
The latest email to the team member using gmail SMTP. 

## About Me ##
Hi, my name Vaibhav Ubale, I have 4.5 years of expiriance in Autimaton.My Skillset is Java, Selenium, Java,Rest Assured,Postman

## Testing Coverage ##
1. Happy Flow Testing
2. Negative Testing and Edge Case Testing
3. Token Testing
4. Data driven Testing with CSV
5. Schema validation

## Tech Stack ##
1. Postman
2. NodeJs 22v
3. Newman
4. Newman-Reporter-htmlextra
5. Github Actions
6. Gmail SMTP
7. Github pages
8. CSV for Data Driven Testing
9. AWS-EC2 for self hosted github runner.

## Github pages ##
You can directly view the latest test report of postman test at the github page : https://vaibhavubale27.github.io/Phoenix-Inwarranty-Flow/

## HTML Report ##
 The report will be created in newman folder
 ![Postman Report](https://github.com/vaibhavubale27/Phoenix-Inwarranty-Flow/blob/Static-Branches/Newmanreport.png)

 ## Project Structure ##

 
```
Phoniex Inwarrenty Flow
├─ In-warranty-flow-Collections.postman_collection.json #Collection File
├─ QA.postman_environment.json #Enviroment File
└─ testdata.csv #Test data file

```
 

## How to run project? ##
You can run the project local system for that
1. Clone the project on local system: https://github.com/vaibhavubale27/Phoenix-Inwarranty-Flow
2. Install Node.js and NPM from :https://nodejs.org/en
3. Install Newman using npm install -g newman
4. Install Newman-reporter-htmlextra : npm install -g newman-reporter-htmlextra
5. Run the newman command :
```
   newman run 'In-warranty-flow-Collections.postman_collection.json' \
          -e QA.postman_environment.json \
          -d testdata.csv \
          -r cli,htmlextra \
          --reporter-htmlextra-export ./newman/index.html
```

 
