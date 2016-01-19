# testWikipediaSpock
Sample functional testing of Wikipedia with Spock.

Requeriments:
* Gradle (http://gradle.org/gradle-download).
* ChromeDriver (https://sites.google.com/a/chromium.org/chromedriver/downloads).

Configuration:
* Edit file `testWikipediaSpock/src/test/resources/GebConfig.groovy` and set your ChromeDriver path in:

```
driver = {
	System.setProperty('webdriver.chrome.driver', 'C:\\backup\\tools\\ChromeDriver\\chromedriver.exe')
   new ChromeDriver()
}
```

Running the tests:

```
cd testWikipediaSpock
gradle test
```

Ckecking the result report:

```
testWikipediaSpock/build/reports/tests/index.html
```

You can develop your own specifications (test cases) in `testWikipediaSpock/src/test/groovy`.

Learning about Spock and Geb:
* Spock Framework Reference Documentation (http://spockframework.github.io/spock/docs).
* The Book Of Geb (http://www.gebish.org/manual/current).



[@jmfvarela] (https://twitter.com/jmfvarela)
