# WARNING: MAY NOT BE UP TO DATE

[![](https://jitpack.io/v/io.samourai.code.wallet/bitcoinj.svg)](https://jitpack.io/#io.samourai.code.wallet/bitcoinj)

### Welcome to bitcoinj

The bitcoinj library is a Java implementation of the Bitcoin protocol, which allows it to maintain a wallet and send/receive transactions without needing a local copy of Bitcoin Core. It comes with full documentation and some example apps showing how to use it.

### Technologies

* Java 6 for the core modules, Java 8 for everything else
* [Maven 3+](http://maven.apache.org) - for building the project
* [Orchid](https://github.com/subgraph/Orchid) - for secure communications over [TOR](https://www.torproject.org)
* [Google Protocol Buffers](https://github.com/google/protobuf) - for use with serialization and hardware communications

### Getting started

To get started, it is best to have the latest JDK and Maven installed. The HEAD of the `master` branch contains the latest development code and various production releases are provided on feature branches.

#### Building from the command line

To perform a full build use
```
mvn clean package
```
You can also run
```
mvn site:site
```
to generate a website with useful information like JavaDocs.

The outputs are under the `target` directory.

#### Building from an IDE

Alternatively, just import the project using your IDE. [IntelliJ](http://www.jetbrains.com/idea/download/) has Maven integration built-in and has a free Community Edition. Simply use `File | Import Project` and locate the `pom.xml` in the root of the cloned project source tree.

### This version

This version of bitcoinj was put together for use in Samourai Wallet and Sentinel as it enables signing of mixed inputs (P2PKH and P2SH-P2WPKH). It includes code from the SegWit branch of bitcoinj and GreenBits version of same. It also includes changes to remove Segwit2X DNS seeds as well as all Spongy Castle dependancies (it is 100% Bouncy Castle). 
