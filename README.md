# test-jmh

This project is a simple test of how Java's JMH microbenchmark framework works.

In it, I created 2 implementations of the fibinacci sequence - one iterative and one recursive.  The framework takes care of everything else.

## HowTo

To create this project, I use the jmh archetype for maven.  

```shell
mvn archetype:generate -DgroupId=com.lanouette -DartifactId=test-jmh -DarchetypeGroupId=org.openjdk.jmh -DarchetypeArtifactId=jmh-java-benchmark-archetype
```

To run the test you need to build first.

```shell
mvn clean install
```

Then, run it.

```shell
java -jar target/benchmarks.jar
```

## Details

For more information about JMH see it's page on the OpenJDK site: https://openjdk.java.net/projects/code-tools/jmh/
