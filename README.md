ProjectHub
================

This project is a PHP version of [Brad Frost’s project hub idea](https://github.com/bradfrost/project-hub).



1. [What is a project hub?](#what-is-a-project-hub)
2. [Why would I use a project hub](#why-would-i-use-a-project-hub)
3. [How to Install](#how-to-install)
4. [How to Manage Your Projects](#how-to-manage-your-projects)
4. [How to Contribute](#how-to-contribute)
5. [Author & Community](#author--community)



What is a project hub?
--------

![Screenshot of ProjectHub, an online project timeline](http://s11.postimg.org/53t2o2cmb/screenshot.png)

A project hub is an online project timelines.

It is a tool for keeping track of the progress of a design/development project.
The hub lives online (either publically available or password protected), so that everyone involved in the team has access to it.
Read more about [project hubs on 24 Ways.](http://24ways.org/2013/project-hubs/)



Why would I use a project hub?
--------

The benefits of using a project hub:

- Serves as a centralized place for the project's key design/development materials
- Easily and visually view project progress
- Provides an archive for project artifacts



How to Install
--------

`ProjectHub` use the [Model418 library](http://github.com/Elephant418/Model418) as a storage abstraction layer. So it could be connected to a database instead of the file system.

The dependencies are committed to have a code easy to install, understand and improve.

To start using `ProjectHub` you have to:

1. Deploy [the files](https://github.com/tzi/ProjectHub/archive/v1.1.0.zip) in a folder visible by apache
2. See the sample project data, via your browser, to check if the installation works 
3. Setup your own project data in the `data` folder 



How to Manage Your Projects
--------

The projects are stored as `Yaml` files. Every file in the `data` folder is a different project.

A project is mainly a timeline of project update, which you can join links, like meetings notes or project deliveries.
   
The code below is a project example file:

```json
name: "My first project"
timeline:
    -
        stamp: "August 14th, 2013"
        content: "Kickoff Meeting"
        links:
            "View notes": "#"
            "View demo": "#"
    -
        stamp: "August 9th, 2013"
        content: "Sign contract"
        links:
            "View contract": "#"
    -
        stamp: "August 7th, 2013"
        content: "Initial meeting"
        links:
            "Meeting Notes": "#"
    -
        stamp: "July 13th, 2013"
        content: "Initial contact"
```



How to Contribute
--------

1. Fork the `ProjectHub` repository
2. Create a new branch for each feature or improvement
3. Send a pull request from each feature branch to the **master** branch

If you don't know much about pull request, you can read [the GitHub article](https://help.github.com/articles/using-pull-requests).

All pull requests must follow the [PSR2 standard](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md).



Author & Community
--------

`ProjectHub` is under [MIT License](http://opensource.org/licenses/MIT).  
The project hub idea & the HTML template was created by [Brad Frost](http://bradfrostweb.com/).  
The PHP version was created & maintained by [Thomas ZILLIOX](http://tzi.fr).

[&uarr; top](#readme)