# karate-example
karate example project with graalvm 22.3 java 17

# Steps to reproduce problem
- Install graalvm using sdkman
```
sdk install java 22.3.r17-grl
```
- check java version
```
java -version
openjdk version "17.0.5" 2022-10-18
OpenJDK Runtime Environment GraalVM CE 22.3.0 (build 17.0.5+8-jvmci-22.3-b08)
OpenJDK 64-Bit Server VM GraalVM CE 22.3.0 (build 17.0.5+8-jvmci-22.3-b08, mixed mode, sharing)
```
- execute karate test
```
mvn clean test
```
error message
```
[ERROR] Tests run: 1, Failures: 0, Errors: 1, Skipped: 0, Time elapsed: 0.637 s <<< FAILURE! - in examples.ExamplesTest
[ERROR] testParallel  Time elapsed: 0.632 s  <<< ERROR!
java.lang.IllegalArgumentException: Could not find option with name js.ecmascript-version.
        at examples.ExamplesTest.testParallel(ExamplesTest.java:15)
```
