# **Introduction**

Cucumber BDD framework to test the Jupiter Toys webpage.The framework is designed with data driven to source different sets of test data and Cucumber BDD for Reporting.

# **Demo**

https://youtu.be/aGFSCOmwdNk

# **Requirements**

- Download and Install Java : https://www.java.com/download/ie_manual.jsp
- Download Apache Maven : https://maven.apache.org/download.cgi 
- Download Jenkins : https://www.jenkins.io/download/#downloading-jenkins
- Download and Install IDE of your choice
- Browser driver - Chrome driver exe : https://chromedriver.chromium.org/downloads
(make sure you have your desired browser driver and class path is your user dir folder where your POM file is.
- IDE Plugins for Maven & Cucumber

# **Features**

- Page Object Design Pattern with Selenium PageFactory in Cucumber
- Use of Data Driven Testing in Cucumber using Scenario Outline
- Use of Hooks
- Use of Jenkins/Jenkinsfile to achieve continuous integration
- State context sharing between different step definition files and different scenarios
- Reports

# **Used tools and framework**
- Selenium
- Maven repository
- Cucumber-BDD
- Jenkins

# **Execution**

1. Maven build

 "mvn clean install" or "mvn clean install -U" will execute tests by default and cucumber BDD report can be found under "projectdir\report\index.html"
 ![planit-cmd-snapshot](https://user-images.githubusercontent.com/68452571/222955569-82d31ff1-d75e-4558-9621-f0eee9bf4a7d.png)
 
2. Using IDE

Right click on the TestRunner.java under src\test\java\Runner package and run as JUnit Test
![planit-cucumber-snapshot](https://user-images.githubusercontent.com/68452571/222955589-58f66e62-2f1c-4041-8a02-9376d121b042.png)

3. Using Jenkins

Setup Jenkins locally and create a pipleine job to configure selenium git repository to trigger build 
![planit-jenkins-snapshot](https://user-images.githubusercontent.com/68452571/222955668-24592447-79ba-4a57-883f-ae07a80d2633.png)
![planit-jenkins-report-snapshot](https://user-images.githubusercontent.com/68452571/222955674-8103893e-a62a-49e2-ac44-e4d889a90265.png)
