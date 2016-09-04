
This Test Automation Framework is created using Java, Selenium Web Driver, TestNG. It can be used across different web based applications.
In this approach, the aim is to build a lot of applications independent reusable keyword components so that they can directly used for another web application without spending any extra effort. 
With the framework in place, whenever we need to automate a web based application, we will not need to start from scratch, but use the application independent keyword components to the extent possible and create application specific components for the specific needs.

  Prerequisites
---------------
*	Java jdk-1.8 or higher
*	Apache Maven 3 or higher
*---------------
* 	

There are 5 different environment configurations [dev, local, qa, stage, and prod]
*	Use -P[environment_id] to copy the respective properties file to //config/env.properties 

  Execution:
---------------
*	Clone the repository.
*	Open command prompt and go to web-test directory.
*	To run on local environment use command ....\.\Selenium-TestNG-Automation-Framework> mvn clean test -Pdev

<p><a href="https://github.com/bravehart84/Selenium-Automation-Framework/wiki/Logging"><h2>Logging:</h2></a></p>

*	log4j configured to capture the test execution logs
*	Configuration file is located at //config/log4j.xml


  Screenshots:
---------------
*	Most of the time we want to Capture Screenshot in WebDriver when some kind of error or exception surfaces while practicing testing, to resolve the same the framework has a method. 
*	getScreenshot() is used to indicate to driver to capture a screenshot and store it in //screenshot/packageName directory.

  Reporting
---------------
*  The framework produces an index.html report. It resides in the same 'target\surefire-reports' folder. This reports gives the link to all the different component of the TestNG reports like Groups & Reporter Output. On clicking these will display detailed descriptions of execution.
*  You can find emailable-report.html from target\surefire-reports to email the test reports. As this is a html report you can open it with browser.
