# sciter-sdk
Sciter is an embeddable HTML/CSS/scripting engine, Windows, Mac OSX and Linux.

# log file
[logfile.htm](https://rawgit.com/c-smile/sciter-sdk/master/logfile.htm)

# Some screenshots of real life applications that use Sciter UI

![WarThinder](https://sciter.com/screenshots/slide-wt5.png)

![Norton Internet Security](https://sciter.com/screenshots/slide-norton-nis.png)

![Avast](https://sciter.com/screenshots/slide-avast.png)

![Cardio monitor](https://sciter.com/screenshots/slide-cardio.png)

# Hello World

* ["hellowest Hello World in the World"](https://sciter.com/tutorials/hello-world-tutorial/) - this demo does not require any compilation. 
* [hello C++ world](https://sciter.com/hello-cpp-tutorial/) - C++ integration demo that shows:
  * how to create HTML/CSS window from C++ code;
  * how to define native C++ function to be called from script;
  * how to use resources embedded as resource.cpp file - generated by bin/packfolder[.exe] utility that compresses folder with HTML/CSS/script files into a static byte array.
  
# Information

* [Application Architecture](https://sciter.com/sciter-ui-application-architecture/)
* [General Sciter embedding principles](https://sciter.com/developers/embedding-principles/) and for [native programmers]( https://sciter.com/developers/for-native-gui-programmers/)
* [Notes for Web Frontend developers](https://sciter.com/developers/for-web-programmers/)

# Essential integration headers

* [include/sciter-x-dom.hpp](include/sciter-x-dom.hpp) - `sciter::dom::element` C++ class pretty much all you need to access DOM tree of the window. That is C++ wrapper of [include/sciter-x-dom.h](plain C DOM API)
* [include/sciter-x-window.hpp](include/sciter-x-window.hpp) - `sciter::window` C++ class represents sciter window on all supported platforms. The window class:  
  * [include/sciter-x-host-callback.h](include/sciter-x-host-callback.h) application (window host) callback interface that handles resource loading and script call methods
  * [include/sciter-x-behavior.h](include/sciter-x-behavior.h) DOM event handler - receiver of DOM events (button clicks, input change events, etc).
  
# Application demos

* [usciter](demos/usciter) - demo "browser" for all supported platforms - use it to load samples from /samples/ folder.
* [uminimal](demos/uminimal) - minimalistic multiplatform integration sample.
* [notepad](demos/notepad) sources of https://html-notepad.com application.
* [notes](demos/notes) sources of https://notes.sciter.com - Sciter Notes application.







