# Release notes 1.3 #

## Backward incompatible changes ##
`Awaitility.callTo` has been renamed to `Awaitility.to` which should be used together with the new `untilCall` method. I.e. instead of writing:
```
await().until( callTo(myObject).myMethod(), equalTo(2) ); // Syntax up until Awaitility 1.2.1
```

you write
```
await().untilCall( to(myObject).myMethod(), equalTo(2) ); // Syntax Awaitility 1.3
```

## Other notable changes ##
  * Awaitility now supports field suppliers using the new `fieldIn` construct, e.g.:
```
await().until(fieldIn(myObject).ofType(int.class), equalTo(2));
```
  * Awaitility now has [Scala](Scala.md) support:
```
await until { myObject.myMethod == 2 }
```

## Minor changes ##
Refer to the [change log](http://github.com/jayway/awaitility/raw/master/changelog.txt).