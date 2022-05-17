# **QA Buddy Program**
## **Table of Contents**
- [Introduction](#introduction)
- [Goals](#goals)
- [Getting Started](#getting-started)
- [Tech Stack](#tech-stack)
- [Frontend Project](#frontend-project)
  - [Frontend Automation Tasks](#fronted-automation-tasks)
- [Backend Project](#backend-project)
  - [Backend Automation Tasks](#backend-automation-tasks)
- [Project's Presentation](#projects-presentation)
- [References](#references)
- [FAQ](#faq)

## **Introduction**
This repository is meant to be used as a checklist for the buddies and mentees in order to have a standard structure across all the projects.

Please create a new repository inside the Wizeline's Organization and follow the instructions listed below:
## **Goals**
- Implement a design pattern and structured folders for frontend automation.
  - Page Object Model.
- Use different levels of documentation.
  - README.md [file](https://www.makeareadme.com/).
  - Comments inside code.
- Use best practices for element selectors.
  - Avoid absolute selectors.
  - Unique selectors.
  - Use different selectors supported.
- Use Eslint for static analysis and assure code standards.
- Coding best practices.
  - Code Abstraction.
  - Naming conventions for method, classes and tests.
  - Avoid hardcoded data.
  - Avoid magic numbers.
  - Descriptive name for test scripts.
  - Avoid explicit waits. (if possible).
  - Hooks.
- Best practiced for Assertions.
  - Single assertion per test.
  - Avoid assertions on the page objects.
- Proper Data management
  - Usage of data providers
  - Usage of .env/config files (when possible) for sensible data.
- Implement an automated reporter.
- Include a .gitignore file.
- Implement Backend Automation.
- Integration with CI/CD tools from [references](#references) section.
- Set up Slack notifications once a new build is done.
-  Implement BrowserStack for cross platform/browser testing.(Ask your buddy for BS credentials or contact eduardo.contreras)
- Create a Slides presentation describing your project, integration of tools, advantages, disadvantages, structure and also include a diagram flow.

>Note: Remember to generate your [Onboarding](https://docs.google.com/spreadsheets/d/1D6KpKeOgf80cQcmw2iOkWNwXv9UYA4hFhUm9Dr97Uhk/edit#gid=0) sheet file for a visual tracking of your process.

## **Getting Started**
* As a starter point it is recommended to install [Homebrew](https://brew.sh/) to help you with the tool installation process.
* Also, we require to download and install [node](https://nodejs.org/en/download/).

    To see if Node is installed, type in `node -v` Terminal.

    To see if NPM is installed, type in `npm -v` Terminal.

*  You need to create a env file the .zshrc file (in case there is no .zshrc file refer to [FAQ](#faq) section.):

    ```bash
    open -e ~/.zshrc
    ```

* Configure your terminal to increase your productivity. You can use the following post as a [suggestion](https://ivanaugustobd.medium.com/your-terminal-can-be-much-much-more-productive-5256424658e8).

## **Tech Stack**
As a suggestion for an IDE:

- [VSCode](https://code.visualstudio.com/)
- [Atom](https://atom.io/)
- [WebStorm](https://www.jetbrains.com/webstorm/)
- [IntelliJ IDEA](https://www.jetbrains.com/idea/)
## **Frontend Project**
1. Initialize a new npm project and install all required dependencies.
2. Navigate to [Todoist](https://todoist.com/) and create an account, get familiar with the site since we are using it for the whole challenge.
3. Implement your code using Page Object Model.
4. Use any of the recommended frameworks from the [references](#references) section.

> Note: We strongly suggest to use a new framework to grain experience and expend your knowledge on new automation tools.

### Fronted Automation Tasks:
- Successful login.
  - Define a test case that performs a successful login, using credentials stored preferably in a .env file
- Unsuccessful login. 
  - Define multiple negative scenarios for login.
- Create a new task. 
  - Create a new task and validate it was created correctly.
- Create 10 new tasks. 
  - Create 10 new tasks and validate they were created correctly. 
  - Task Names should be dynamic.

## **Backend project**
1. Navigate to [Todoist API](https://developer.todoist.com/rest/v1/)
2. Download [Postman](https://www.getpostman.com/)
3. Define a new collection and a new environment for your variables

> Note: We recommend to use Postman and Newman for those beginners on API testing because these tools offer a GUI, if you are more experienced we suggest you explore any other backend automation tool from the [references](#references) section.

### Backend Automation Tasks:
1. Get your authorization token and save it as an environment variable.
2. Create a new folder inside your collection for projects and another one for tasks. 
3. Create the following endpoints and its corresponding Tests: status codes, content, json schema,response time, etc.    
  a) Projects:
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
4. Create Negative scenarios for each endpoint.
5. Integrate one framework for API Test Automation i.e.
  *[Newman](https://www.npmjs.com/package/newman)
  So you can run your tests from the command line.


## **Project's presentation**
The presentation is aimed to make the mentee to experiment a role play making a proposal with the client on a testing architecture, explaining What and Why was it designed that way.
The presentation must contain at least thw following points:
* QA process that is going to be followed.
* Git workflow to be used.
* Testing types and their benefits.
* Listed used tools and why they were selected.
* Diagram of the selected tools and their interactions.

Sections:
1. Formal presentation in English - 30 min.
2. Technical demo and project explanation - 30 min.

> Note: The presentation is about your proposal simulating you are a new QA joining the Todoist project. Also, remember to record your demo, it saves time, avoid any last minute failure and it is easier to explain using a video.

The following slides can be used as a template so the mentee has a general overview about how the presentation should look. However, the final presentation is not restricted to contain only the structure provided there. It is expected that the mentee proposes the narrative and information that needs to be presented.

* [Template](https://docs.google.com/presentation/d/1BP7S7dtIsJL9HrXRKy5YhxWi74N8LicCByP2MTCTepw/edit?ts=609afddb#slide=id.gcaaa55f3fe_0_39)


## **References**
Frontend Javascript based frameworks:
* [Testcafe](https://devexpress.github.io/testcafe/)
* [Cypress](https://www.cypress.io/)
* [Playwright](https://playwright.dev/)
* [WebdriverIO](https://webdriver.io/)
* [Nightwatch](https://nightwatchjs.org/api)
* [Protractor](https://www.protractortest.org/#/)

Device farms:
* [BrowserStack](https://www.browserstack.com/)
* [SauceLabs](https://saucelabs.com/)

CI tools:
* [Jenkins](https://jenkins.io/)
* [Github Actions](https://github.com/features/actions)
* [CircleCI](https://circleci.com/)
* [Travis CI](https://travis-ci.org/)

Static analysis:
* [ESLint](https://eslint.org/)
* [SonarQube](https://www.sonarqube.org/)

Reporter:
* [Slack Reporter](https://kb.itglue.com/hc/en-us/articles/228469048-Setting-up-Slack-webhook-notifications)
* [Allure](http://allure.qatools.ru/)

Backend:
* [Postman](https://www.getpostman.com/)
* [Supertest](https://github.com/visionmedia/supertest)
* [Mocha & Chai](https://www.paradigmadigital.com/dev/testeo-api-rest-mocha-chai-http/)
* [Newman](https://www.npmjs.com/package/newman)
* [Artillery](https://artillery.io/)
* [K6](https://github.com/loadimpact/k6)
* [Axios](https://github.com/axios/axios)

Test Strategies:
* [Test Plan](https://sites.google.com/wizeline.com/wizelineqa/home)

Metrics Monitoring for Performance:
* [DataDog](https://www.datadoghq.com/)

## **FAQ**
Q1) How do I create a .zshrc file?

A1) Follow the instructions described in this [post](https://superuser.com/questions/886132/where-is-the-zshrc-file-on-mac).