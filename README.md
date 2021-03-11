# REACTOS STARFIELD  SCREENSAVER

This is Starfield Screensaver for Windows and ReactOS, an OpenGL accelerated screensaver that simulates an animated space field.
It requires hardware acceleration for working with minimal CPU usage.
It works on Windows 9x/ME/NT4.0/2000/XP/Vista/7/8/8.1/10, both 32 bit and 64 bit platforms are supported.

![The screensaver in action](doc/common/example.jpg)

## BUILDING FROM SOURCES

CMake is used for building the program with MinGW or Visual Studio.
After you downloaded the sources, by cloning the repository or after unpacking the ZIP file of the stable version, run the command:

cmake <path_to_sources>

After the configuration process completed, you can start the build by running tipically `make` or `ninja`, or open the solution file with Visual Studio.

## INSTALLATION

Just copy the executable of the screen saver under `%systemroot%\system32` and the help files under `%systemroot%\help`.
Perhaps, the next step will be an installer to automate this process...

## NOTES FOR USERS WITH GMA ADAPTER

It looks like that the video driver of Intel HD graphics adapters disables all OpenGL acceleration and it switches to software rendering, but JUST when you launch screensavers.

From: http://www.intel.com/support/graphics/sb/CS-004684.htm

> Hardware acceleration for OpenGL screensavers is not enabled in the graphics drivers because of potential compatibility issues with a number of third party OpenGL screensavers. Running the screensavers in software mode should reduce the possibility of system lockups or crashes while these screen savers are enabled. This should not prevent these screen savers from running, but slow rendering speed may be seen. This does not affect OpenGL-based games or general applications.

A fast workaround, rename the screensaver form .scr to .sCr. from this tip:

http://uktsupport.ipbhost.com/index.php?showtopic=11194


## CLOSING WORDS

Have fun with ReactOS Starfield Screensaver!

-------------------------------------------------------------------
Carlo Bramini, 12-02-2012

