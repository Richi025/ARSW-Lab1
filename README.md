# Introduction to Maven, GIT, GitHub

ARSW Laboratory No. 1, in which the console use of Maven, GIT and GITHub is practiced.

## Starting

To get the project you can use the command 

git clone https://github.com/Richi025/ARSW-Lab1.git

if you want to run the application use the command.

```
java -cp target/miprimera-app-1.0-SNAPSHOT.jar edu.escuelaing.ar
sw.ASE.app.App
```

### Previous requirements

You need to have Maven and Java installed, preferably in their latest versions.

```
Download Maven in http://maven.apache.org/download.html 

Follow the instructions in http://maven.apache.org/download.html#Installation
```
```
Download Java in https://www.java.com/es/download/ie_manual.jsp
```

### Installing

### Previous requirements

You need to have Maven and Java installed, preferably in their latest versions.

```
Download Maven at http://maven.apache.org/download.html 

Follow the instructions at http://maven.apache.org/download.html#Installation
```
```
Download Java at https://www.java.com/es/download/ie_manual.jsp
```

### Installing

1. Open an OS Shell

2. Go to the directory where you will store your projects, with the following command.

```
mvn archetype:generate -DgroupId=edu.escuelaing.arsw.ASE.app -DartifactId=myfirst-app -DarchetypeArtifactId=maven-archetype-quickstart -
DinteractiveMode=false
``` 

3. Enter the project folder.

```
cd myprimera-app/
```

4. To view the source code of the App, enter the /app folder.

```
For Windows

type App.java
```

5. Then exit to the root folder and use the command to package.

```
mvn package
```

6. Now to run the app use the command.

```
java -cp target/miprimera-app-1.0-SNAPSHOT.jar edu.escuelaing.ar
sw.ASE.app.App
```

7. To generate the documentation, enter the POM.xml file and add the following.

```
  <reporting>
    <plugins>
      <plugin>
        <groupId>org.apache.maven.plugins</groupId>
	<artifactId>maven-javadoc-plugin</artifactId>
	<version>2.10.1</version>
      </plugin>
    </plugins>
   </reporting>
  <build>
    <plugins>
      <plugin>
	<groupId>org.apache.maven.plugins</groupId>
	<artifactId>maven-javadoc-plugin</artifactId>
	<version>2.10.1</version>
      </plugin>
    </plugins>
   </build>
```
8. Now run the following commands in console:

```
mvn javadoc:javadoc
mvn javadoc:jar
mvn javadoc:aggregate
mvn javadoc:aggregate-jar
mvn javadoc:test-javadoc
mvn javadoc:test-jar
mvn javadoc:test-aggregate
mvn javadoc:test-aggregate-jar
```

9. Now by entering the following path you will be able to see the project documentation and open the index.html file

```
\miprimera-app\target\apidocs
```

## Built with

* [Maven](https://maven.apache.org/) - Dependency management
* [java](https://www.java.com/es/) - Programming language

## Versioned

We use [Git](https://github.com/) for version control. For available versions, see the tags in this repository. 

## Authors

* **Jose Ricardo Vasquez Vega** - [Richi025](https://github.com/Richi025)


## License

This project is licensed under the GNU license; See the [LICENSE.txt](LICENSE.txt) file for details.

