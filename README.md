# Example of broken tests using Phantomjs

This is a slightly modified slimmed down version of [https://github.com/sjrd/scala-js-example-app](https://github.com/sjrd/scala-js-example-app)
[Scala.js](http://www.scala-js.org/).


## Running the test command will give the following error  

```
[info] 1/2     example.ScalaJSExampleTest.ScalaJSExample		Success
[info] 2/2     example.ScalaJSExampleTest		Success
java.util.concurrent.TimeoutException: Futures timed out after [4841340619 nanoseconds]
	at scala.concurrent.impl.Promise$DefaultPromise.ready(Promise.scala:219)
	at scala.concurrent.impl.Promise$DefaultPromise.result(Promise.scala:223)
	at scala.concurrent.Await$$anonfun$result$1.apply(package.scala:107)
	at scala.concurrent.BlockContext$DefaultBlockContext$.blockOn(BlockContext.scala:53)
	
[error] (test:executeTests) java.util.concurrent.TimeoutException: Futures timed out after [4841340619 nanoseconds]
[error] Total time: 21 s, completed Oct 31, 2016 10:28:42 AM
...
```
