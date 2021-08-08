# junit5-jupiter-starter-gradle-kotlin

[JUnit 5](http://junit.org/junit5) is the latest version of the well-known JUnit test framework. Unlike its predecessor, JUnit 5 is modularized and composed of several modules:
```
JUnit 5 = JUnit Platform + JUnit Jupiter + JUnit Vintage
```
The JUnit Platform serves as a foundation for launching testing frameworks on the JVM. JUnit Jupiter is the combination of the new [programming model](http://junit.org/junit5/docs/current/user-guide/#writing-tests) and [extension model](http://junit.org/junit5/docs/current/user-guide/#extensions) for writing tests and extensions in JUnit 5. JUnit Vintage provides a `TestEngine` for running JUnit 3 and JUnit 4 based tests on the platform.


## Example
[Calculator.kt](src/main/kotlin/com/example/project/Calculator.kt)

[CalculatorTests.kt](src/test/kotlin/com/example/project/CalculatorTests.kt)

Run `./gradlew test` to execute all tests.

Output:

```bash
> Task :test

CalculatorTests > divisionByZeroError() PASSED

CalculatorTests > add(int, int, int) > com.example.project.CalculatorTests.add(int, int, int)[1] PASSED

CalculatorTests > add(int, int, int) > com.example.project.CalculatorTests.add(int, int, int)[2] PASSED

CalculatorTests > add(int, int, int) > com.example.project.CalculatorTests.add(int, int, int)[3] PASSED

CalculatorTests > add(int, int, int) > com.example.project.CalculatorTests.add(int, int, int)[4] PASSED

CalculatorTests > 1 + 1 = 2() PASSED

BUILD SUCCESSFUL in 34s
3 actionable tasks: 3 executed
```

## Reference
[junit5-samples](https://github.com/junit-team/junit5-samples) repo.
[Gradle's native JUnit Platform support](https://docs.gradle.org/current/userguide/java_testing.html#using_junit5)
