# Starter for Angular Quarkus Web Project

## Setup

To set up a new project start changing the Maven groupId and artifactId on every pom.xml file :
* [main pom](pom.xml)
* [frontend pom](frontend/pom.xml)
* [backend pom](backend/pom.xml)
* [distribution pom (for parent and dependencies)](distribution/pom.xml)

Set Java and Quarkus version in the properties of the [main pom](pom.xml)

And Node version in the properties of the [frontend pom](frontend/pom.xml)

## Maven commands
### Run dev
Tu run the app in dev mode
```shell script
mvn compile quarkus:dev
```
This will build the frontend app, and start running Quarkus in dev mode.

To just run Quarkus in dev mode without updating the frontend app (faster to launch)
```shell script
mvn :quarkus:dev
```

### Install

```shell script
mvn install
```
This will create an uber jar of the project at distribution/target/

### Clean
```shell script
mvn clean
```