# mvnrepository
General repository for maven

## Usage
pom.xml:
```xml
    <repositories>
        <repository>
            <id>hengyunabc-maven-repo</id>
            <url>https://raw.githubusercontent.com/clearriver/mvnrepository/master</url>
        </repository>
    </repositories>
or
    <repositories>
        <repository>
            <id>hengyunabc-maven-repo</id>
            <url>https://raw.github.com/clearriver/mvnrepository/master</url>
        </repository>
    </repositories>
```
## mvn deploy  (maven-metadata.xml & ojdbc14-10.2.0.5.0.jar will be created at local maven project)
```xml
mvn deploy:deploy-file -DgroupId=com.oracle -DartifactId=ojdbc14 -Dversion=10.2.0.5.0 -Dpackaging=jar -Dfile=D:\river\mvnrepository\com\oracle\ojdbc14\10.2.0.5.0\ojdbc14-10.2.0.5.0.jar
```

## mvn install  (maven-metadata-local.xml will be created at local maven repository)
```xml
mvn install:install-file -DgroupId=com.oracle -DartifactId=ojdbc14 -Dversion=10.2.0.5.0 -Dpackaging=jar -Dfile=D:\river\mvnrepository\com\oracle\ojdbc14\10.2.0.5.0\ojdbc14-10.2.0.5.0.jar
```
