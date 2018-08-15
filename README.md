

# Backend Automation  



## Setup Project


Follow below steps to setup the project in Eclipse :-

* Install _**Maven plugin**_ in Eclipse if it is not supported by your current version.


* Import _**beAutomation**_ project directory into Eclipse.



## Run Project

Follow below steps to run the project in Eclipse :-

* Right click on the project, then click on _**Run As**_, then click on _**Maven build...**_

* To run the complete test suite, paste the below command into _**Goals**_ field.

 ```
 clean compile exec:java -Dexec.mainClass="main.OptimizerTestCase" test
 ```


* To run only failed test cases, paste the below command into _**Goals**_ field.

```
test -DsuiteXmlFile=target/surefire-reports/testng-failed.xml
```


* To create the allure report, paste the below command into _**Goals**_ field.

```
site
```



## Report Paths

**Allure report path** = `target/allure-report/index.html`  

**TestNg report path** = `target/surefire-reports/emailable-report.html`

