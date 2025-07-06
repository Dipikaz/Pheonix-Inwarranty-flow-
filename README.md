# Postman API Automation Integration with Github Actions #

  This repository is a demonstration for POC for integrating postman tests with github actions. The Tests are written in Postman and they are executed on VM eith the help pf Newman and Newman-Reporter-Htmlextra.
  Github Actions will trigger the project execution on every push to main branch. You can also execute the project manually using workflow_dispatch. The Projects runs on scheduled time with help of 
  cron job.

  The HTML report is archieved and kept in the artifact section for the team to download it. Along with that they can view the report directly from github page: https://dipikaz.github.io/Pheonix-Inwarranty-flow-/.
  The latest report is mailed to the team members using GMAIL SMPT.


## About Me ##
Hi! My name is Dipika Zope. I have 2.5 years of experience in Automation Testing. My skillset include UI Automation with Selenium Webdriver, Cypress, Playwright and for API testing I have used Rest Assured and Postman.
You can connect with me over : ![LinkedIn](www.linkedin.com/in/dipika-zope-967766225)


## Testing Coverage ##
1. Happy Flow testing
2. Negative Testing and Edge case testing
3. Token Testing
4. Data Driven Testing with CSV
5. Schema Validation
6. Secrets management with Github Secrets



## Tech Stack ##

1. Postman
2. Nodejs 22v
3. Newman
4. Newman-Reporter-Htmlextra
5. Github Actions
6. Gmail SMTP
7. Github Pages
8. CSV for Data Driven Testing
9. AWS-EC2 Instance for Self Hosted Github Runner
   
## GitHub Pages ##
You can directky view the latest test report of the Postman test on GitHub page link: https://dipikaz.github.io/Pheonix-Inwarranty-flow-/.

## HTML Report ##
The Report will be created in newman folder
![Postman Report](https://github.com/Dipikaz/Pheonix-Inwarranty-flow-/blob/static-content/Html%20report.png)

## Project Structure ## 
Pheonix Inwarranty Flow
1. Inwarranty-flow Collection.postman_collection.json  ##Collection file
2. QA.postman_environment.json   ## Environment File
3. testData.csv   ##Test data file

## How to run the Project ##
You can run the project on your local system for that:
1. Clone the Project on locat system : https://github.com/Dipikaz/Pheonix-Inwarranty-flow-.git
2. Install Nodejs and NPM: https://nodejs.org/en/download
3. Install Newman using  ''' npm install -g newman ''' 
4. Install Newman-reporter-htmlextra npm install -g newman-reporter-htmlextra
5. Run the Newman command:
         '''
             newman run 'Inwarranty-flow Collection.postman_collection.json' \
            -e 'QA.postman_environment.json' \
            -d 'testData.csv' \
            -r cli,htmlextra \
            --reporter-htmlextra-export ./newman/index.html
        '''

           





     
