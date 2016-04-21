Simple archetype to create a Java application with a main method which does a request to the commercetools platform.

It prints the product names and the category names it is in:

```
found product MB PREMIUM TECH T in categories Long sleeves
found product MB SOFTSHELL LINER in categories Snowboard equipment
found product WB ATHLETIC TANK in categories Tank tops
found product GIRLS HARTBREAK CREW in categories Long sleeves
found product SAPPHIRE in categories Snowboard equipment
```

Create the software project
----------------
requirements:
* install [Java 8](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
* install [Maven 2+](https://maven.apache.org)
* a commercetools platform project


```bash
mvn archetype:generate -B \
  -DarchetypeGroupId=com.commercetools.maven-archetypes \
  -DarchetypeArtifactId=commercetools-hello-java-archetype \
  -DarchetypeVersion=0.1.1 \
  -DgroupId=io.sphere.demo \
  -DartifactId=commercetools-hello-java \
  -Dversion=0.1.0-SNAPSHOT \
  -DcommercetoolsProjectKey=YOUR-PROJECT-KEY \
  -DcommercetoolsClientId=YOUR-CLIENT-ID \
  -DcommercetoolsClientSecret=YOUR-CLIENT-SECRET
```

Change to the project folder
----------------------------
```bash
cd commercetools-hello-java
```

Run the project
----------------

```bash
mvn compile exec:java
```
