# Spring Boot Java Kotlin Archetype

Spring Boot Java Kotlin Archetype is a Maven Archetype that help to generate a Maven Spring Boot project that can work with Java and Kotlin.

# Usage

```shell
mvn archetype:generate \
  -DarchetypeGroupId=io.github.nicholassiew1991 \
  -DarchetypeArtifactId=spring-boot-java-kotlin-archetype \
  -DarchetypeVersion=1.2.0 \
  -DgroupId={groupId} \
  -DartifactId={artifactId} \
  -Dversion={version} \
  -Dpackage={package} \
  -DspringBootVersion={springBootVersion} \
  -DwebProject=true
  -DjavaVersion={javaVersion} \ 
  -DkotlinVersion={kotlinVersion}
```