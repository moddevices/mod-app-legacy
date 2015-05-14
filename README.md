mod-app
=======

This is a work-in-progress desktop application of the MOD interface and backend,<br/>
natively integrated in the OS (no external web browser needed).<br/>

In order to run this application you need to have ingen and mod-ui installed system-wide.<br/>

If you're using the KXStudio repositories, run this command to install all dependencies:<br/>
`sudo apt-get install ingen mod-ui phantomjs python3-pyqt5 python3-pyqt5.qtsvg python3-pyqt5.qtwebkit`<br/>

If you're not using the KXStudio repositories, you'll need to clone mod-ui inside the sources/modules folder.<br/>
Then install these dependencies to get almost everything running:
```
sudo apt-get install ingen phantomjs jack-capture sndfile-tools<br/>
sudo apt-get install python3-pyqt5 python3-pyqt5.qtsvg python3-pyqt5.qtwebkit<br/>
sudo apt-get install python3-rdflib python3-bson python3-pil python3-pystache python3-pymongo<br/>
sudo apt-get install python3-serial python3-tornado python3-whoosh<br/>
```
And finally you'll need the latest lilv (version 0.22 or SVN) with python3 bindings enabled.

After you're done installing the dependencies, simply type:<br/>
`make`<br/>
To generate the necessary resource files to be able to run mod-app (and mod-remote).

You can now run mod-app using:<br/>
`./source/mod-app`<br/>

Binary builds will be available at a later date.


mod-remote
==========

This is a work-in-progress application that allows you to connect to a remote MOD device.<br/>
The only required dependency for it is PyQt.

Binary builds for Windows and MacOS are available, see the releases section on GitHub.
