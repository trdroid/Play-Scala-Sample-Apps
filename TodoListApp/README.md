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

*TodoListApp/app/controllers/Application.scala*

```scala
package controllers

import play.api.mvc._

object Application extends Controller {

  def index = Action {
    Ok(views.html.main())
  }

}
```

*TodoListApp/app/views/main.scala.html*

```scala
<!DOCTYPE html>

<html>
    <head>
        <title>Just Play Scala</title>
    </head>
    <body>
        <h1>Just Play Scala</h1>
    </body>
</html>
```

*TodoListApp/conf/application.conf*

```conf
# This is the main configuration file for the application.
# ~~~~~

# Secret key
# ~~~~~
# The secret key is used to secure cryptographics functions.
# If you deploy your application to several instances be sure to use the same key!
application.secret="kY9oA[`V9q1]5467cTQao4EHb@xFHZA5^b:at[;:nLEvdWYpBnchCneh>P?u0Wp_"

# The application languages
# ~~~~~
# application.langs="en"

# Global object class
# ~~~~~
# Define the Global object class for this application.
# Default to Global in the root package.
# application.global=Global

# Router
# ~~~~~
# Define the Router object to use for this application.
# This router will be looked up first when the application is starting up,
# so make sure this is the entry point.
# Furthermore, it's assumed your route file is named properly.
# So for an application router like `my.application.Router`,
# you may need to define a router file `conf/my.application.routes`.
# Default to Routes in the root package (and conf/routes)
# application.router=my.application.Routes

# Database configuration
# ~~~~~
# You can declare as many datasources as you want.
# By convention, the default datasource is named `default`
#
# db.default.driver=org.h2.Driver
# db.default.url="jdbc:h2:mem:play"
# db.default.user=sa
# db.default.password=""

# Evolutions
# ~~~~~
# You can disable evolutions if needed
# evolutionplugin=disabled

# Logger
# ~~~~~
# You can also configure logback (http://logback.qos.ch/),
# by providing an application-logger.xml file in the conf directory.

# Root logger:
logger.root=ERROR

# Logger used by the framework:
logger.play=INFO

# Logger provided to your application:
logger.application=DEBUG
```

*TodoListApp/conf/routes*

```conf
# Routes
# This file defines all application routes (Higher priority routes first)
# ~~~~

# Home page
GET     /                           controllers.Application.index

# Map static resources from the /public folder to the /assets URL path
GET     /assets/*file               controllers.Assets.versioned(path="/public", file)
```

*TodoListApp/project/build.properties*

```properties
#Activator-generated Properties
#Thu Sep 01 10:56:48 EDT 2016
template.uuid=71358ad9-fc02-4dfa-aa4a-1ae1964e5181
sbt.version=0.13.5
```

*TodoListApp/project/plugins.sbt*

```properties
resolvers += "Typesafe repository" at "http://repo.typesafe.com/typesafe/releases/"

addSbtPlugin("com.typesafe.play" % "sbt-plugin" % "2.3.4")
```

*TodoListApp/build.sbt*

```sbt
name := """TodoListApp"""

version := "1.0-SNAPSHOT"

lazy val root = project.in(file(".")).enablePlugins(PlayScala)
```

### Running the default project

```sh
:~/onBB/Play-Scala-Sample-Apps/TodoListApp$ activator run
[info] Loading project definition from /home/droid/onBB/Play-Scala-Sample-Apps/TodoListApp/project
[info] Updating {file:/home/droid/onBB/Play-Scala-Sample-Apps/TodoListApp/project/}todolistapp-build...
[info] Resolving org.fusesource.jansi#jansi;1.4 ...
[info] Done updating.
[info] Set current project to TodoListApp (in build file:/home/droid/onBB/Play-Scala-Sample-Apps/TodoListApp/)
[info] Updating {file:/home/droid/onBB/Play-Scala-Sample-Apps/TodoListApp/}root...
[info] Resolving org.fusesource.jansi#jansi;1.4 ...
[info] Done updating.

--- (Running the application from SBT, auto-reloading is enabled) ---

[info] play - Listening for HTTP on /0:0:0:0:0:0:0:0:9000

(Server started, use Ctrl+D to stop and go back to the console...)

```

**Making a request from the browser**

Requesting the following URL in the browser "http://localhost:9000/" displays the following in the console

```sh
(Server started, use Ctrl+D to stop and go back to the console...)

[info] Compiling 4 Scala sources and 1 Java source to /home/droid/onBB/Play-Scala-Sample-Apps/TodoListApp/target/scala-2.10/classes...
[warn] Error reading API from class file : java.lang.UnsupportedClassVersionError: controllers/routes$javascript : Unsupported major.minor version 52.0
[warn] Error reading API from class file : java.lang.UnsupportedClassVersionError: controllers/routes : Unsupported major.minor version 52.0
[warn] Error reading API from class file : java.lang.UnsupportedClassVersionError: controllers/routes$ref : Unsupported major.minor version 52.0
[info] play - Application started (Dev)
```

and displays the following in the browser

![](_misc/Output%20in%20browser.png)
