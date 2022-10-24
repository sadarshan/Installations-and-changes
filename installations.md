[This](https://youtu.be/mKt4ZTaE2bk) video instructions explains clearly about the installation instructions and errors that I found and resolved. I highly recommend to follow the instructions for errorless installation.

---

[gazebo installation instructions](https://classic.gazebosim.org/tutorials?tut=install_ubuntu)

**changes in commands:** 

    gazebo11        -> gazebo
    libgazebo11-dev -> libgazebo-dev



Download/clone PX4-Autopilot GitHub for SITL from [here](https://github.com/PX4/PX4-Autopilot)

After cloning, open terminal in PX4-Autopilot and run ```make px4_sitl gazebo``` to start building binaries for copter.

> **NOTE:** If you don't have cmake in your OS, easiest way to install it from *Ubuntu Software* app. Just search *cmake* and install the package. `#ffffff`

Found issue while building cmake: 
```
- Checking for module 'gstreamer-1.0 >= 1.0'
--   No package 'gstreamer-1.0' found
-- Checking for module 'gstreamer-base-1.0 >= 1.0'
[ 91%] Built target systemcmds__tune_control
--   No package 'gstreamer-base-1.0' found
-- Checking for module 'gstreamer-app-1.0 >= 1.0'
--   No package 'gstreamer-app-1.0' found
```

tried resolving it using [these](https://askubuntu.com/questions/384059/error-compiling-a-package-configure-error-no-gstreamer-1-0-1-0-0) commands. [One more Similar solution](https://stackoverflow.com/questions/25558308/error-no-gstreamer-1-0-1-4-0-gstreamer-found)

---

[QGC installation instructions](https://docs.qgroundcontrol.com/master/en/getting_started/download_and_install.html)

