Every S60-Devices, that has Python and the PythonScriptingShell enabled, provides a "Bluetooth console", which allows you to get a interactive Python-shell for the phone on a remote host, which is a PyC-hardcoded feature and wasn't working nor flexible enough for me.
So here is a lightweight alternative for this: 2 scripts (and a symbian-s60-compiled program), one for the phone and one for the pc.
The phone-script acts as a daemon, advertising the "PyBlueShell"-Service with flexible authorisation and the pc offers a console-client for the remote shell and a gui to choose the device.
In the future the phone-side-script will be offered as sis-application, that runs all the time in the Background.

**Attention:**
  * the scripts are currently in Beta-State and have been tested on a Nokia E70, PyS60 v.1.9.5 from (see below)
  * the pc-side-script requires the "lightblue"-module from (see below) and the "PyBluez"-Module from (see below)

**the Project makes use of:**
  * Python Module: Lightblue from http://lightblue.sourceforge.net/
  * Python Module: PyBluez from http://code.google.com/p/pybluez/
  * Python Library (already included): StandOut from http://www.voidspace.org.uk/python/standout.html
  * Python for S60 / PyS60 (latest unofficial build) from https://garage.maemo.org/projects/pys60/