![http://github.com/jayway/awaitility/raw/master/resources/Awaitility_logo_red_small.png](http://github.com/jayway/awaitility/raw/master/resources/Awaitility_logo_red_small.png)
<br />
<br />
Testing asynchronous systems is hard. Not only does it require handling threads, timeouts and concurrency issues, but the intent of the test code can be obscured by all these details. Awaitility is a DSL that allows you to express expectations of an asynchronous system in a concise and easy to read manner. For example:

```
@Test
public void updatesCustomerStatus() throws Exception {
    // Publish an asynchronous event:
    publishEvent(updateCustomerStatusEvent);
    // Awaitility lets you wait until the asynchronous operation completes:
    await().atMost(5, SECONDS).until(costumerStatusIsUpdated());
    ...
}
```

## News ##
  * 2014-11-28: [Awaitility 1.6.3](http://dl.bintray.com/johanhaleby/generic/awaitility-1.6.3.zip) is released. See [change log](http://github.com/jayway/awaitility/raw/master/changelog.txt) for details.
  * 2014-10-15: [Awaitility 1.6.2](http://dl.bintray.com/johanhaleby/generic/awaitility-1.6.2.zip) is released with improved support for [Condition Evaluation Listeners](Usage#Condition_Evaluation_Listener.md), [Groovy 2.3 Trait support](Groovy#Groovy_2.3_and_above.md) and [deadlock detection](Usage#Deadlock_detection.md). See [change log](http://github.com/jayway/awaitility/raw/master/changelog.txt) for more details.
  * 2014-07-03: [Awaitility 1.6.1](http://dl.bintray.com/johanhaleby/generic/awaitility-1.6.1.zip) is released with support for [Condition Evaluation Listeners](Usage#Condition_Evaluation_Listener.md) as well as various bug fixes. See [change log](http://github.com/jayway/awaitility/raw/master/changelog.txt) for more details.
[Older news](OldNews.md)

## Documentation ##
  * [Getting started](Getting_started.md)
  * [User Guide](Usage.md)
  * [Awaitility Javadoc](http://awaitility.googlecode.com/svn/tags/1.6.3/apidocs/com/jayway/awaitility/Awaitility.html)

<br>
<br>
<hr />
<h2>Founded by:</h2>
<a href='http://www.jayway.com'><img src='http://www.arctiquator.com/oppenkallkod/assets/images/jayway_logo.png' /></a>

<h2>Other open source projects:</h2>
<a href='http://www.powermock.org'>
<img src='http://powermock.googlecode.com/svn/trunk/src/site/resources/images/logos/powermock.png' width='219' height='100' /></a>
<a href='http://rest-assured.googlecode.com'><img src='http://rest-assured.googlecode.com/svn/trunk/rest-assured-logo-green.png' /></a><br>