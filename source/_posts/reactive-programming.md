---
title: What is Reactive programming
date: 2020-08-31 11:18:11
tags: ['Programming']
---
**Reactive programming** *is a* [programming paradigm](https://en.wikipedia.org/wiki/Programming_paradigm) *oriented around* [data flows](https://en.wikipedia.org/wiki/Dataflow_programming) *and the propagation of change. This means that it should be possible to express static or dynamic data flows with ease in the programming languages used, and that the underlying execution model will automatically propagate changes through the data flow*.

In the short description:

**Reactive programming is programming with asynchronous data streams.**

We can imagine data streams like below image.

![Data Stream](data_streams.gif)
source: atom.io



A stream is a sequence of ongoing events ordered in time. It can emit three different things: a value (of some type), an error, or a "completed" signal.








In a way, this isn't anything new. Event buses or your typical click events are really an asynchronous event stream, on which you can observe and do some side effects. Reactive is that idea on steroids. You are able to create data streams of anything, not just from click and hover events. Streams are cheap and ubiquitous, anything can be a stream: variables, user inputs, properties, caches, data structures, etc. For example, imagine your Twitter feed would be a data stream in the same fashion that click events are. You can listen to that stream and react accordingly.

**On top of that, you are given an amazing toolbox of functions to combine, create and filter any of those streams.** That's where the "functional" magic kicks in. A stream can be used as an input to another one. Even multiple streams can be used as inputs to another stream. You can *merge* two streams. You can *filter* a stream to get another one that has only those events you are interested in. You can *map* data values from one stream to another new one.

If streams are so central to Reactive, let's take a careful look at them, starting with our familiar "clicks on a button" event stream.







### When apply Reactive Programing ###

* Compare 
* Configuration
* Dependencies
* Database configuration
* How to run tests
* Deployment instructions

### How to apply Reactive Programing ###

* Writing tests
* Code review
* Other guidelines

### Sample application ###

* Repo owner or admin

* Other community or team contact

### Conclusion