# qa-buddy-program
This repository is ment to be used as a checklist for the buddies and mentees in order to have a standard structure across all the projects.

Please fork this repository and follow the instructions listed below:

## Goals
* Implement Page Object Model with the of the Javascript based frameworks listed
* Use best practices for element selectors
* Use Eslint for static analysis and ensure code standards
* Configure SonarQube (Optional)
* Configure Jenkins to build on demand
* Set up Slack notifications one a new build is done
* Implement BrowserStack for cross platform/browser testing
* Create a Slides presentation describing your project, integration of tools, adventages, disadvantages, structure and also include a diagram flow. 

## Front-end project
* Init a npm project and install all required dependencies (eg, framework, reporters).
* Navigate to [Todoist](https://todoist.com/) and create an account, get familiar with the site since we are using it for the whole challenge.
* Implement your code using Page Object Model
### Fronted Automation Tasks:
- [ ] Successful login. Define a test case that performs a successful login, using credentials stored preferably in a .env file
- [ ] Unsuccessful login. Define multiple negative scenarios for login.
- [ ] Create a new task. Create a new task and validate it was created correctly
- [ ] Create 10 new task. Create 10 new task and validate they were created correctly. Task Names should be dynamical.


## Back-end project
* Navigate to [Todoist API](https://developer.todoist.com)
* Download [Postman](https://www.getpostman.com/)
* Create an environment
* Create a collection 

## References
Front-end Javascript based frameworks:
* [Testcafe](https://devexpress.github.io/testcafe/)
* [Nightwatch](https://nightwatchjs.org/api)
* [WebdriverIO](https://webdriver.io/)

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
