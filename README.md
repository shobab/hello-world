

# Backend Automation  



## Setup Project


Follow below steps to setup the project in Eclipse :-

* Install _Maven plugin_ in Eclipse if it was not supported by your current version.


* Import _beAutomation_ project directory into Eclipse.



## Run Project

Follow below steps to run the project in Eclipse :-

* Right click on the project, then click on _Run As_, then click on _Maven build..._

* To run the complete test suite, paste the below command into _Goals_ field.

 ```
 clean compile exec:java -Dexec.mainClass="main.OptimizerTestCase" test
 ```


* To run only failed test cases, paste the below command into _Goals_ field.

```
test -DsuiteXmlFile=target/surefire-reports/testng-failed.xml
```


* To create the allure report, paste the below command into _Goals_ field.

```
site
```



## Report Paths

**Allure report path** = `target/allure-report/index.html`  

**TestNg report path** = `target/surefire-reports/emailable-report.html`

