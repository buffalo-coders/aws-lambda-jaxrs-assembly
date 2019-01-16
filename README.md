# org.buffalo-coders:aws-lambda-jaxrs-assembly

Apache Maven Assembly Plugin assembly descriptor useful for AWS Lambda JAX-RS projects.

## Usage

Leverage this via the `maven-assembly-plugin` execution:

```xml
  <build>
    <plugins>
      <plugin>
        <artifactId>maven-assembly-plugin</artifactId>
        <dependencies>
          <dependency>
            <groupId>org.buffalo-coders.aws.lambda.jaxrs</groupId>
            <artifactId>assembly</artifactId>
            <version>1</version>
          </dependency>
        </dependencies>
        <executions>
          <execution>
            <phase>package</phase>
            <goals>
              <goal>single</goal>
            </goals>
            <configuration>
              <descriptorRefs>
                <descriptorRef>lambda</descriptorRef>
              </descriptorRefs>
            </configuration>
          </execution>
        </executions>
      </plugin>
    </plugins>
  </build>
```

## Status

[![Build Status](https://travis-ci.com/buffalo-coders/aws-lambda-jaxrs-assembly.svg?branch=master)](https://travis-ci.com/buffalo-coders/aws-lambda-jaxrs-assembly)
