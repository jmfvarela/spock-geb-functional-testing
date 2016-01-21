Proof of concept: functional testing with Spock and Geb.

Tested in Windows.

# Requirements
* Gradle (http://gradle.org/gradle-download).
* ChromeDriver (https://sites.google.com/a/chromium.org/chromedriver/downloads).

# Configuration
* Edit file `spock-geb-functional-testing/src/test/resources/GebConfig.groovy` and set your ChromeDriver path in:
```
driver = {
	System.setProperty('webdriver.chrome.driver', 'C:\\backup\\tools\\ChromeDriver\\chromedriver.exe')
   new ChromeDriver()
}
```

# Running tests
```
cd spock-geb-functional-testing
gradle test
```

# Result report
```
spock-geb-functional-testing/build/reports/tests/index.html
```

# Developing your tests
You can develop your own test cases (named specifications in Spock) in `spock-geb-functional-testing/src/test/groovy`.

# Learning about Spock and Geb
* Spock Framework Reference Documentation (http://spockframework.github.io/spock/docs).
* The Book Of Geb (http://www.gebish.org/manual/current).
