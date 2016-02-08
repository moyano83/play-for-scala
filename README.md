#Play for Scala
This is a repository created to hold the exercises and examples of the book Play for Scala writen by Peter Hilton, Erik Bakker and Francisco Canedo.

## CHAPTER 1: Introduction to Play 2.
To create a new play project, use `activator new <project_name>`.You can run an application from the command line typing `activator ~run`
- app: Application source code
- conf: Configuration files and data
- project: Project build scripts
- public: Publicly accessible static files
- test: Automated tests

In play, Controller classes handles Actions that return results. Routing configuration is stored in `conf/routes`. Here you define the url and the method of the class that would intercept it.
`GET     /                                controllers.Application.index`
You can start a console to get a scala cli that allows you to test methods without having a server running. To to that type:
```
$ activator console
scala>views.html.hello.render("Hello!")
```

## CHAPTER 2: Your first Play application
Internationalization files are stored under `conf/` with names _<messages>[.<language>]_ the last bit is appended for non default bundles.
