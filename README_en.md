[Leia em Português do Brasil](https://github.com/williamcanin/gosync-pug/blob/master/README.md)

# Go!Sync Pug

[![NodeJS with Gulp](https://github.com/williamcanin/gosync-pug/actions/workflows/npm-gulp.yml/badge.svg)](https://github.com/williamcanin/gosync-pug/actions/workflows/npm-gulp.yml)

Simple boilerplate using [Pug](http://pugjs.org), [Twitter Bootstrap](http://getbootstrap.com), [Gulp](http://gulpjs.com/) and [Browser Sync](https://www.browsersync.io).

### Intro

**Go!Sync Pug** makes it easy to develop HTML's projects in a way that the monitoring of all changes in Pug, Stylesheets and Javascripts are made automatically through tasks [Gulp](http://gulpjs.com/), [plugins](https://github.com/williamcanin/gosync-pug/blob/master/package.json) and the [Browser Sync](https://www.browsersync.io). To forget the F5 on browser ;)


### *How it works the operation of **Go!Sync Pug**?*

* All .pug structure are minified.

* You create style sheets with "SASS" that will be compiled for "CSS" and automatically minificadas every change.

* JavaScripts are concatenated and automatically diminished every change also.

* Images are also minified, however, only at startup Browser Sync or performing compilation with the `$ gulp build` or task ` gulp imagemin`.

* The project will be stored in the folder `build`.


### Requirements

| Required       | Version | Checking      | How to install  |
| --------------- | -------| ------------------- | -------------- |
| Git             | indifferent | `git --version`     | [Git](http://git-scm.com/) |
| Node            | >= 12.0 | `node -v`          | [Nodejs](http://nodejs.org/) |
| Python          | >= 3.5    | `python --version`  | [Python](https://www.python.org/) |
| Npm             | indifferent | `npm --version`     | **Nodejs** contains **Npm** |
| Gulp            | >=4.0.0  | `gulp -v`           | [Gulp](http://gulpjs.com/) |


> See the documentation for each application to install.


### Installing

After installing all of the above requirements, do the following commands:

* 1 - Make Clone **Go!Sync Pug** and go to the folder:

~~~
$ git clone https://github.com/williamcanin/gosync-pug.git "mysite"; cd mysite
~~~

* 1 - Installing the **Go!Sync Pug** dependencies:

~~~
$ npm install
~~~

### Compiling

* Use the command below to compile your project:

~~~
$ gulp build
~~~

or

~~~
$ $(npm bin)/gulp build
~~~

Note: Your site will be compiled into the `public` folder.

### Starting local server

* The following command launches a local server with [Browser Sync](https://www.browsersync.io) (for development):

~~~
$ gulp serve
~~~

or

~~~
$ $(npm bin)/gulp serve
~~~

> Note 1: For more gulp tasks, use `gulp --tasks`.
> Note 2: No need to compile and then start the server.

### Development

* 1 - You should create any layout structure for your project in the `src/templates` directory using [Pug](http://pugjs.org).

* 2 - The `src/views` folder is where you should create your pages, which will have includes, extends and         blocks through the `src/templates/includes` and `src/templates/layouts` folders.

* 3 -  Before hosting your project on the server, change in `config.json` the value of `url`, by placing the url of your site. After that, you can run the `gulp build` command and host.

### Donation

If you liked my work, buy me a coffee :coffee: :smiley:

[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=YBK2HEEYG8V5W&source)

### License

[MIT License](https://opensource.org/licenses/MIT) © William Canin