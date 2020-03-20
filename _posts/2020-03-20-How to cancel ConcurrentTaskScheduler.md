---
layout: post
title: How to cancel ConcurrentTaskScheduler
---

```java
ConcurrentTaskScheduler taskScheduler = new ConcurrentTaskScheduler();

Runnable task = new Runnable() {};

ScheduledFuture scheduledFuture = taskScheduler.schedule(task, cronJobTrigger);

schedulFuture.cancel();
```

This is no ```shutdown()``` method for ```ConcurrentTaskScheduler``` , but the scheduler will return a ```ScheduledFuture```, which has a ```cancel()``` method, with a boolean ```mayInterruptIfRunning``` argument.
