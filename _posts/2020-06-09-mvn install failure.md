---
layout: post
title: mvn install failure
---

```java
mvn clean install
```

throws

```java
[ERROR] Failed to execute goal org.apache.maven.plugins:maven-compiler-plugin:3.8.1:compile (default-compile) on project demo: Fatal error compiling: error: invalid target release: 1.11 -> [Help 1]
```

<url>https://github.com/carlossg/docker-maven/issues/117</url>

### Problem

```java
<properties>
	<java.version>1.11</java.version>
</properties>
```

### Solution

```java
<properties>
	<java.version>11</java.version>
</properties>
```

From JDK 9 onwards, the 1.x prefix was dropped.
