# QA Buddy Program
This repository is meant to be used as a checklist for the buddies and mentees in order to have a standard structure across all the projects.

Please create a new repository inside the Wizeline's Organization and follow the instructions listed below:

## Goals
* Implement Page Object Model with the of the Javascript based frameworks listed for Frontend Automation.
* Document everything, add readme describing the steps and how to's on each section.
* Use best practices for element selectors.
* Use Eslint for static analysis and assure code standards.
* Configure SonarQube .
* Implement Backend Automation.
* Configure any of the described CI tools mentioned below to build on demand.
* Set up Slack notifications once a new build is done.
* Implement BrowserStack for cross platform/browser testing.(Ask your buddy for BS credentials or contact eduardo.contreras)
* Create a Slides presentation describing your project, integration of tools, adventages, disadvantages, structure and also include a diagram flow.


## Frontend project
* Initialize a new npm project and install all required dependencies.
* Navigate to [Todoist](https://todoist.com/) and create an account, get familiar with the site since we are using it for the whole challenge.
* Implement your code using Page Object Model

### Fronted Automation Tasks:
- [ ] Successful login. Define a test case that performs a successful login, using credentials stored preferably in a .env file
- [ ] Unsuccessful login. Define multiple negative scenarios for login.
- [ ] Create a new task. Create a new task and validate it was created correctly
- [ ] Create 10 new tasks. Create 10 new tasks and validate they were created correctly. Task Names should be dynamic.


## Backend project
* Navigate to [Todoist API](https://developer.todoist.com/rest/v1/)
* Download [Postman](https://www.getpostman.com/)
* Define a new collection and a new environment for your variables

### Backend Automation Tasks:
1. Get your authorization token and save it as an environment variable
2. Create a new folder inside your collection for projects and another one for tasks. 
3. Create the following endpoints and its corresponding Tests: status codes, content, json schema,response time, etc.    
  a) Projects
    * Get all projects
    * Create a new project
    * Get a project
    * Update a project
    * Delete a project

    b) Tasks:  
   * Get active tasks  
   * Create a new task  
   * Get an active task  
   * Update a task  
   * Close a task  
   * Reopen a task   
   * Delete a task
4. Create Negative scenarios for each endpoint
5. Integrate [Newman](https://www.npmjs.com/package/newman), so you can run your tests from the command line 

### How to choose a Frontend Framework?

  A useful, short and happy guide to help you choose between some open source frameworks based on JS.
   * What? 
   * Why?
   * How?

  https://docs.google.com/document/d/1TdCpuQ5ZsCOB9NDBkg1LApez7ob_6BykKwfi1H63Di4/edit?usp=sharing
 
 PS: the document include links to POC's for the frameworks tackled on the reading.

## Project's presentation
The presentation is aimed to make the mentee to experiment a role play making a proposal with the client on a testing architecture, explaining What and Why was it designed that way.
The presentation must contain at least thw following points:
* QA process that is going to be followed.
* Git workflow to be used.
* Testing types and their benefits.
* Listed used tools and why they were selected.
* Diagram of the selected tools and their interactions.

## Frontend Project Stage 2:
#### Note: Available only after completing all the previous work mentioned above.

### Frontend Challenge Stage 2 will try to cover as much of the following:

#### Tasks
* Create a New Tas
  * Type a due date
  * Select Today as due date
  * Select Tomorrow as due date
  * Select Next Week as due date
  * Select No Date
  * Select a specific day in the calendar
  * Add a specific hour to be completed
  * Update Time Zone
  * Select a specific project while creating a new task
  * Set priority for a new Task
* Create N Number of Tasks
* Create N number of Sub Tasks
* Create Task Above
* Create Task Below
* Edit Task
* Drag and Drop Task

#### Projects
* Create a New Project
  * Select project color
  * Add to Favorites (on/off)
* Enter to a Project
  * Add a Section
  * Create N number of Tasks inside a new section
  * Sort Tasks by Name
  * Sort Tasks by Priority
  * Sort Tasks by Date
  * Show Completed Tasks

## References
Frontend Javascript based frameworks:
* [Testcafe](https://devexpress.github.io/testcafe/)
* [Cypress](https://www.cypress.io/)
* [Nightwatch](https://nightwatchjs.org/api)
* [WebdriverIO](https://webdriver.io/)
* [Protractor](https://www.protractortest.org/#/)

Device farms:
* [BrowserStack](https://www.browserstack.com/)
* [SauceLabs](https://saucelabs.com/)

CI tools:
* [Jenkins](https://jenkins.io/)
* [Travis CI](https://travis-ci.org/)
* [CircleCI](https://circleci.com/)

Static analysis:
* [ESLint](https://eslint.org/)
* [SonarQube](https://www.sonarqube.org/)

Reporter:
* [Slack Reporter](https://kb.itglue.com/hc/en-us/articles/228469048-Setting-up-Slack-webhook-notifications)
* [Allure](http://allure.qatools.ru/)

Backend:
* [Postman](https://www.getpostman.com/)
* [Newman](https://www.npmjs.com/package/newman)

Test Strategies:
* [Test Plan](https://sites.google.com/wizeline.com/wizelineqa/home)
