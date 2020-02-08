# Example of publishing a JAR with Codefresh

This is a Git repository that holds a Java library. It also has a settings.xml Maven file for uploading the jar to artifactory/nexus.

## Packaging the library

To compile the jar run:

```bash
mvn package
```

## Publish the jar

To publish the JAR file, edit settings.xml with your package manager credentials and the pom.xml with your package manager URL. Then run

```bash
mvn -s settings.xml deploy
```

and then visit your package manager


## To use this project in Codefresh

There is also a [codefresh.yml](codefresh.yml) for easy usage with the [Codefresh](codefresh.io) CI/CD platform.

More details can be found in [Codefresh documentation](https://codefresh.io/docs/docs/learn-by-example/java/publish-jar/).

