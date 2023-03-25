# Using Cucumber in a Kotlin Gradle project

This is a minimal setup for using the Cucumber BDD tool for projects based on Kotlin and Gradle.    



## Requirements

* Java 17 and Gradle 7.6 have been used for this setup. It is likely that other versions will work just as well, but they have not been tested.



## Getting Started

Run the following commands:

```bash
git clone https://github.com/crispy-coding/kotlin-gradle-cucumber-setup.git
cd kotlin-gradle-cucumber-setup
gradle test
```

The tests should run successfully and produce the file `build/cucumber-report.html`. This can be opened in a browser to see the results of the test. To see what happens if a test fails, simply uncomment the `fail()` command in `src/test/kotlin/features/TodayFridayTests.kt` and rerun the tests.

The setup can be imported into IntelliJ so that the tests can be executed through its GUI by running the `CucumberTestRunner.kt`, or the tests can be run directly in the `is_it_friday_yet.feature` file.



## References

These are helpful sources that have been used to get this setup up and running, including copying code:

* [10 Minute Tutorial](https://cucumber.io/docs/guides/10-minute-tutorial/?lang=java) from the official website.
* [Kukumber-Skeleton](https://github.com/mlvandijk/kukumber-skeleton) which provides a setup for Kotlin and Cucumber, but Maven instead of Gradle.
* [Cucumber-Java-Skeleton](https://github.com/cucumber/cucumber-java-skeleton) which provides a setup for Gradle and Cucumber, but Java instead of Kotlin.
* [Using Cucumber with Gradle](https://www.baeldung.com/java-cucumber-gradle) guide by Baeldung, but using Java instead of Kotlin.