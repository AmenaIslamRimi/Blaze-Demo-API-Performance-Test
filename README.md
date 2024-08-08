# Blaze-Demo-API-Performance-Test
# Objectives
The Blaze Demo website allows testers to explore web UI interactions within a travel context. Testers can ensure a seamless user journey from choosing the departure city to the destination city. 
# Prerequisites
* JDK (Latest LTS)
* Set environment for java JAVA-HOME
* Jmeter
* Set environment for JMeter JMETER-HOME
# How to run
## Execute following commands
* git clone <repo_url>
* ./jmeter (For Linux)
* or, .jmeter (For Windows)
# How to generate the report
## For JMeter 5.1.1 version or higher
To generate the report in Non-GUI mode, execute the test using the below command:
* For Windows: jmeter -n -t yourFile.jmx -l yourFile.csv -e -o Reports
* For Linux: ./jmeter.sh -n -t yourFile.jmx -l yourFile.csv -e -o Reports
### Generate a report with JMeter
* Thread groups > add > listener > Aggregate report
* In Aggregate report: Create filename 'filename.csv'
* (Top navbar) Tools > Generate HTML report > browse 'filename.csv' > browse 'user.properties' > give (empty folder) output directory
* Click Generate report
For both options, the output folder contains the generated report in HTML format at the end of the test.
# Tests Conducted
## Load Test
Load testing determined how the API performs under expected user loads. The test aimed to identify response times, throughput, and potential bottlenecks.
## Stress Test
Stress testing was executed to determine the API's behavior under extreme conditions. The test helps identify the point at which the API fails or experiences significant performance degradation. 
## Capacity Analysis
Capacity analysis was conducted to establish the maximum number of requests the API can handle before its performance becomes unacceptable or fails.
# Documents
## Excel Reports 
[Load Test Report](https://docs.google.com/spreadsheets/d/1pYAoIpGEb_EHAUOTT92bM8J8491LJ9cXrYsOCohB-Ug/edit?gid=0#gid=0) <br />
[Stress Test Report](https://docs.google.com/spreadsheets/d/1zs3X1GruiEEEtWEgHERFnL91Eag3_byHORlrZSYNCMw/edit?gid=0#gid=0)
# Results 
## Screenshots
![Load Test](https://i.postimg.cc/8PF7KVQD/load-test-report.png) <br />
![Stress Test](https://i.postimg.cc/d3gVPLPF/stress-test-report.png) 
