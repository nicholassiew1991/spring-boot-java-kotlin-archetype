# Spring Boot Java Kotlin Archetype

Spring Boot Java Kotlin Archetype is a Maven Archetype that help to generate a Maven Spring Boot project that can work with Java and Kotlin.

# Usage

## Configure Maven Settings

Add following configuration to `${user.home}/.m2/settings.xml`
```xml
<settings>

  <profiles>
    <profile>
      <id>github</id>
      <repositories>
        <repository>
          <id>github</id>
          <url>https://maven.pkg.github.com/nicholassiew1991/spring-boot-java-kotlin-archetype</url>
          <snapshots>
            <enabled>true</enabled>
          </snapshots>
        </repository>
      </repositories>
    </profile>
  </profiles>

  <activeProfiles>
    <activeProfile>github</activeProfile>
  </activeProfiles>
  
</settings>
```

## Generate Project

Run the following command to generate the project

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