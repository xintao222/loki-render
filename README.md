# Loki Render

Loki Render allows you to create your own render farm, serving Blender render jobs to a group of computers. Loki is easy to setup and runs on Linux, Windows or Mac, making it a quick and flexible distributed network rendering solution!

This is a fork of the original project by Daniel Petersen over on [Sourceforge](https://sourceforge.net/projects/loki-render/) 

## Getting Started

Loki Render can be launched with a simple command:

```
java -jar LokiRender-<version>.jar [<BlenderExe>] [MasterIP]
```

* Replace <version> to match the jar file you have
* Add the full path to the Loki Render jar file if you wish to run the command outside the directory where the jar is stored
* Use [<BlenderExe>] by adding the path to a Blender executable, to start Loki Render in grunt mode without the GUI (great for headless rendering)
* Use [<MasterIP>] to specify the IP address of a server running Loki Render in Master mode, otherwise Loki Render will attempt to auto detect

Examples:
```
java -jar LokiRender-071-1.jar
java -jar LokiRender-071-1.jar /path/to/blender
java -jar LokiRender-071-1.jar 192.168.17.45
java -jar LokiRender-071-1.jar /path/to/blender 192.168.17.45
java -jar /path/to/jar/folder/LokiRender-071-1.jar /path/to/blender 192.168.17.45
```

### Prerequisites

This repo is mainly tested with OpenJDK version 8, but could work on other versions as well. It is tested mainly on Linux, but should also work on Windows and Mac as well.

### Installing

Simply copy the jar file somewhere, and run the command above.

### And coding style tests

TO-DO

## Contributing

Please feel free to send bug fixes and improvements for consideration. I may not be able to put much time into this project, so it needs support from the community.

## Wish LIst

I have the following ideas for future upgrades

* Make command line arguments more specific/verbose
* New Mode: "Client", which can connect to a "Master" and add jobs. Authentication would be a good idea at this point
* HTTP/Web interface for "Master" mode GUI. I am personally much more comfortable coding GUI's in HTML/CSS/JS/JQuery than Java
* After "Client' mode has been added, and "Master" mode has a web based GUI, the "Master" mode should be able to run without Java's GUI, so it can be placed on a headless server as well
* Hmmm maybe I should somehow move this into the support ticket area, lol

## Versioning

We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/mikeperalta1/loki-render/tags). 

## Authors

* **Daniel Petersen** - *Initial work* - [Original Project](https://sourceforge.net/projects/loki-render/)
* **Mike Peralta** - *Reviving bug fix and fork to this repo* - [Music](http://MikePeralta.com/)

See also the list of [contributors](https://github.com/mikeperalta1/loki-render/contributors) who participated in this project.

## License

This project is licensed under the GPL v3 License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Huge thanks to Daniel Petersen for creating this wonderful and fun project in the first place, and giving his blessing for this fix+fork to happen
* The wonderful people working on Blender
* My dog


