# Sentiment Analysis of Tweets in Polyglot Native

This demo shows how we can use JVM libraries in a native project. This example uses Klaxon (Kotlin) to parse tweets, Open NLP (Java) to do sentiment analysis of tweets, and Scala collections to correlate tweets with time series. The tweets in the example are the tweets that contain a word "Ethereum" and the time series is the price of cryptocurrency Ether on the market.

To compile the demo make sure you have Scala, Kotlin, and GraalVM installed and `$SCALA_HOME`, `$KOTLIN_HOME`, and `$GRAALVM_HOME` set. Then simply invoke
```
./polyglot-compile.sh
```

This will build two native images:
1) `sentimentsC` is the native program that combines C, Java, Scala, and Kotlin.
2) `sentimentsJava` is the native program that combines only the JVM languages. It is build only for debugging with `gdb` on OS X.
