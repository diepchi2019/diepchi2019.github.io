---
title: What is Subject in RxJs 
date: 2020-09-30 16:03:33
tags: ['Programming', 'Reactive Programming']
---
**What is subject ?**

Subjects is a an special type of Observable.It allows multicasted value to many Observer object. While Observable only allow unicast.

```
A Subject is like an Observable. but can multiple cast to many Observers. Subjects are like EventEmiter: they maintain a registry of many listerners.
```

Internally to the Subject, subscribe does not invoke a new execution that delivers values. It simply registers the given Observer in a list of Observers, it's same with to how add listener usually works in other libraries.

Example:

```
import { Subject } from 'rxjs';
 
const subject = new Subject<number>();
 
subject.subscribe({
  next: (v) => console.log(`observerA: ${v}`)
});
subject.subscribe({
  next: (v) => console.log(`observerB: ${v}`)
});
 
subject.next(1);
subject.next(2);
 
// Logs:
// observerA: 1
// observerB: 1
// observerA: 2
// observerB: 2
```

**The types of Subject**

There are also a few specializations of the `Subject` type: `BehaviorSubject`, `ReplaySubject`, and `AsyncSubject`.

