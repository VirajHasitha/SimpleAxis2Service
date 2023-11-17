# SimpleAxis2Service

This project contains the source code of a simple Axis2Service which can be used to health check WSO2 servlet transport port 9443. 

## Build Instructions
- Navigate to the directory where the pom.xml resides.
- Execute commond 
       mvn clean install -Dmaven.test.skip=true

Target contains the following files
- healthcheck.aar
- healthcheck-1.0.0.jar

## Deployment Instructions
- Add the healthcheck.aar file into the <WSO2AM_HOME>/repository/deployment/server/axis2services/ directory.
- Add the healthcheck-1.0.0.jar file into the <WSO2AM_HOME>/repository/components/lib/ directory.

HealthCheck endpoint can be access via the following URL.
https://localhost:9443/services/HealthCheck
