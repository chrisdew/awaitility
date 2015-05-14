# Installation #

## Java DSL ##
Maven:

```
<dependency>
      <groupId>com.jayway.awaitility</groupId>
      <artifactId>awaitility</artifactId>
      <version>1.6.3</version>
      <scope>test</scope>
</dependency>
```

Gradle:
```
compile 'com.jayway.awaitility:awaitility:1.6.3'
```

## Scala DSL ##
Maven:
```
<dependency>
      <groupId>com.jayway.awaitility</groupId>
      <artifactId>awaitility-scala</artifactId>
      <version>1.6.3</version>
      <scope>test</scope>
</dependency>
```

SBT:
```
val awaitility-scala = "com.jayway.awaitility" % "awaitility-scala" % "1.6.3"
```

Gradle:
```
compile 'com.jayway.awaitility:awaitility-scala:1.6.3'
```

## Groovy DSL ##
Maven:
```
<dependency>
      <groupId>com.jayway.awaitility</groupId>
      <artifactId>awaitility-groovy</artifactId>
      <version>1.6.3</version>
      <scope>test</scope>
</dependency>
```

Grapes:
```
@Grapes(
    @Grab(group='com.jayway.awaitility', module='awaitility-groovy', version='1.6.3')
) 
```

Gradle:
```
compile 'com.jayway.awaitility:awaitility-groovy:1.6.3'
```

## Non-Maven / Gradle users ##
Download [Awaitility](http://dl.bintray.com/johanhaleby/generic/awaitility-1.6.3.zip) and put it in your class-path. You may also need to download the [third-party dependencies](http://dl.bintray.com/johanhaleby/generic/awaitility-dependencies.zip) and put them in your classpath as well. Scala users must also download [awaitility-scala](http://dl.bintray.com/johanhaleby/generic/awaitility-scala-1.6.3.zip) and Groovy users must download [awaitility-groovy](http://dl.bintray.com/johanhaleby/generic/awaitility-groovy-1.6.3.zip).

# Documentation #
When you've successfully downloaded and configured Awaitility in your classpath please refer to the [user guide](Usage.md) for examples.