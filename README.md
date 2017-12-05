# Live555
Fork from [Live555 official websit](http://www.live555.com/).
Version 2017.10.28.

---
## Windows Compile

1. open live555/Win/live555.sln by vs2015(or vs2017).
2. modify "WindowsTargetPlatformVersion" value to "**10**" for each sub-project if u're using **Win10**.
3. u're done, run it :)

---
## Linux Compile
nothing specilal with [official guide](http://www.live555.com/liveMedia/#config-unix).

1. generate Makefile in each sub-directory.
    ``` shell
    cd live555
    sudo chmod 777 ./genMakefiles
    ./genMakefiles linux
    ```

2. want to change output-path?(default output to **/usr/local**) modify "PREFIX = /path/to/output" in file "Makefile.head" in each sub-directory. 

3. make it
    ``` shell
    make
    ```