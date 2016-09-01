### Creating the project

**On Windows**

```sh
~/onGit/play-scala-sample-apps (master)
$ which activator
/c/Software/Typesafe-Activator/typesafe-activator-1.3.10/bin/activator

~/onGit/play-scala-sample-apps (master)
$ activator new ToDoList just-play-scala

Fetching the latest list of templates...

[WARN] [09/01/2016 10:12:36.765] [default-akka.actor.default-dispatcher-4] [ActorSystem(default)] Failed to download new template catalog properties: java.lang.IllegalArgumentException: requirement failed: Source file 'C:\Users\droid\.activator\1.3.10\templates\index.db_f7c6b21c7044732a.tmp' is a directory.
[INFO] [09/01/2016 10:12:36.765] [default-akka.actor.default-dispatcher-4] [akka://default/user/template-cache] We have index hash 8a2285c306189290715965bc7fae4399d0d5c882 but haven't downloaded that index - attempting to download it now.
[ERROR] [09/01/2016 10:12:37.233] [default-akka.actor.default-dispatcher-4] [akka://default/user/template-cache] Could not find a template catalog. (java.lang.IllegalArgumentException: requirement failed: Source file 'C:\Users\droid\.activator\1.3.10\templates\index.db_ac2c52046dd3a1a3.tmp' is a directory.
java.lang.IllegalArgumentException: requirement failed: Source file 'C:\Users\droid\.activator\1.3.10\templates\index.db_ac2c52046dd3a1a3.tmp' is a directory.
        at scala.Predef$.require(Predef.scala:224)
        at sbt.IO$.copyFile(IO.scala:637)
        at sbt.IO$.move(IO.scala:839)
        at activator.package$RichIO$.createViaTemporary$extension(package.scala:30)
        at activator.templates.repository.UriRemoteTemplateRepository$$anonfun$resolveIndexTo$1.apply(UriRemoteTemplateRepository.scala:228)
        at activator.templates.repository.UriRemoteTemplateRepository$$anonfun$resolveIndexTo$1.apply(UriRemoteTemplateRepository.scala:220)
        at sbt.IO$.withTemporaryDirectory(IO.scala:344)
        at activator.templates.repository.UriRemoteTemplateRepository.resolveIndexTo(UriRemoteTemplateRepository.scala:220)
        at activator.cache.TemplateCacheActor$$anonfun$9.apply(TemplateCacheActor.scala:165)
        at activator.cache.TemplateCacheActor$$anonfun$9.apply(TemplateCacheActor.scala:163)
        at scala.Option.foreach(Option.scala:257)
        at activator.cache.TemplateCacheActor.preStart(TemplateCacheActor.scala:163)
        at akka.actor.Actor$class.aroundPreStart(Actor.scala:470)
        at activator.cache.TemplateCacheActor.aroundPreStart(TemplateCacheActor.scala:25)
        at akka.actor.ActorCell.create(ActorCell.scala:580)
        at akka.actor.ActorCell.invokeAll$1(ActorCell.scala:456)
        at akka.actor.ActorCell.systemInvoke(ActorCell.scala:478)
        at akka.dispatch.Mailbox.processAllSystemMessages(Mailbox.scala:279)
        at akka.dispatch.Mailbox.run(Mailbox.scala:220)
        at akka.dispatch.Mailbox.exec(Mailbox.scala:231)
        at scala.concurrent.forkjoin.ForkJoinTask.doExec(ForkJoinTask.java:260)
        at scala.concurrent.forkjoin.ForkJoinPool$WorkQueue.runTask(ForkJoinPool.java:1339)
        at scala.concurrent.forkjoin.ForkJoinPool.runWorker(ForkJoinPool.java:1979)
        at scala.concurrent.forkjoin.ForkJoinWorkerThread.run(ForkJoinWorkerThread.java:107)

java.lang.IllegalArgumentException: requirement failed: Source file 'C:\Users\droid\.activator\1.3.10\templates\index.db_ac2c52046dd3a1a3.tmp' is a directory.
        at scala.Predef$.require(Predef.scala:224)
        at sbt.IO$.copyFile(IO.scala:637)
        at sbt.IO$.move(IO.scala:839)
        at activator.package$RichIO$.createViaTemporary$extension(package.scala:30)
        at activator.templates.repository.UriRemoteTemplateRepository$$anonfun$resolveIndexTo$1.apply(UriRemoteTemplateRepository.scala:228)
        at activator.templates.repository.UriRemoteTemplateRepository$$anonfun$resolveIndexTo$1.apply(UriRemoteTemplateRepository.scala:220)
        at sbt.IO$.withTemporaryDirectory(IO.scala:344)
        at activator.templates.repository.UriRemoteTemplateRepository.resolveIndexTo(UriRemoteTemplateRepository.scala:220)
        at activator.cache.TemplateCacheActor$$anonfun$9.apply(TemplateCacheActor.scala:165)
        at activator.cache.TemplateCacheActor$$anonfun$9.apply(TemplateCacheActor.scala:163)
        at scala.Option.foreach(Option.scala:257)
        at activator.cache.TemplateCacheActor.preStart(TemplateCacheActor.scala:163)
        at akka.actor.Actor$class.aroundPreStart(Actor.scala:470)
        at activator.cache.TemplateCacheActor.aroundPreStart(TemplateCacheActor.scala:25)
        at akka.actor.ActorCell.create(ActorCell.scala:580)
        at akka.actor.ActorCell.invokeAll$1(ActorCell.scala:456)
        at akka.actor.ActorCell.systemInvoke(ActorCell.scala:478)
        at akka.dispatch.Mailbox.processAllSystemMessages(Mailbox.scala:279)
        at akka.dispatch.Mailbox.run(Mailbox.scala:220)
        at akka.dispatch.Mailbox.exec(Mailbox.scala:231)
        at scala.concurrent.forkjoin.ForkJoinTask.doExec(ForkJoinTask.java:260)
        at scala.concurrent.forkjoin.ForkJoinPool$WorkQueue.runTask(ForkJoinPool.java:1339)
        at scala.concurrent.forkjoin.ForkJoinPool.runWorker(ForkJoinPool.java:1979)
        at scala.concurrent.forkjoin.ForkJoinWorkerThread.run(ForkJoinWorkerThread.java:107)
```

**On Ubuntu**

```sh
~/onBB/Play-Scala-Sample-Apps$ which activator
/home/droid/software/typesafe-activator/activator-dist-1.3.10/bin/activator

~/onBB/Play-Scala-Sample-Apps$ activator new TodoListApp just-play-scala

Fetching the latest list of templates...

OK, application "TodoListApp" is being created using the "just-play-scala" template.

To run "TodoListApp" from the command line, "cd TodoListApp" then:
/home/droid/onBB/Play-Scala-Sample-Apps/TodoListApp/activator run

To run the test for "TodoListApp" from the command line, "cd TodoListApp" then:
/home/droid/onBB/Play-Scala-Sample-Apps/TodoListApp/activator test

To run the Activator UI for "TodoListApp" from the command line, "cd TodoListApp" then:
/home/droid/onBB/Play-Scala-Sample-Apps/TodoListApp/activator ui

```

### Project structure and content

![](_misc/Project%20Structure.png)
