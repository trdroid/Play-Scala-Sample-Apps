### Creating a new Play application using Activator and a simple template

activator new \<path to app directory\>/\<name of app directory\>  \<name of the template\>

The following creates an app called basicApp in the current working directory 

> $ activator new basicApp just-play-scala

    Fetching the latest list of templates...
    
    OK, application "basicApp" is being created using the "just-play-scala" template.
    
    To run "basicApp" from the command line, "cd basicApp" then:
    /home/droid/scratchpad/Play-Scala/basicApp/activator run
    
    To run the test for "basicApp" from the command line, "cd basicApp" then:
    /home/droid/scratchpad/Play-Scala/basicApp/activator test
    
    To run the Activator UI for "basicApp" from the command line, "cd basicApp" then:
    /home/droid/scratchpad/Play-Scala/basicApp/activator ui
    

Run the project
> $ cd basicApp

> basicApp$ sbt run

    [info] Loading project definition from /home/droid/scratchpad/Play-Scala/basicApp/project
    [info] Updating {file:/home/droid/scratchpad/Play-Scala/basicApp/project/}basicapp-build...
    [info] Resolving org.fusesource.jansi#jansi;1.4 ...
    [info] Done updating.
    [info] Set current project to basicApp (in build file:/home/droid/scratchpad/Play-Scala/basicApp/)
    [info] Updating {file:/home/droid/scratchpad/Play-Scala/basicApp/}root...
    [info] Resolving org.fusesource.jansi#jansi;1.4 ...
    [info] Done updating.
    
    --- (Running the application from SBT, auto-reloading is enabled) ---
    
    [info] play - Listening for HTTP on /0:0:0:0:0:0:0:0:9000
    
    (Server started, use Ctrl+D to stop and go back to the console...)

