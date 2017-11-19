# Multi-Vina #
=============

Multi-vina is modified version of Autodock Vina so you can dock multiple ligands at a time which was not 
possible by the original Autodock Vina. Now you won't need to use vina_split anymore to split the ligands 
as single ligands.

AutoDock Vina is an open-source program for doing molecular docking. It was been designed and implemented by Dr. Oleg Trott in the Molecular Graphics Lab at The Scripps Research Institute. 

Building from Source
--------------------
Attention: Building Multi-Vina from source
Step 1: Install a C++ compiler suite
On Windows, you may want to install Visual Studio; on OS X, Xcode; and on Linux, the GCC compiler suite.

Step 2: Install Boost
Install Boost. Then, build and run one of the example programs, such as the Regex example, to confirm that you have completed this step. If you can't do this, please seek help from the Boost community.

Step 3: Build Vina
If you are using Visual Studio, you may want to create three projects: lib, main and split, with the source code from the appropriate subdirectories. lib must be a library, that the other projects depend on, and main and split must be console applications. For optimal performance, remember to compile using the Release mode.
You can use the Makefiles as they are provided here but may need to change the directories where Boost is installed.

On OS X and Linux, you may want to navigate to the appropriate build subdirectory, customize the Makefile by setting the paths and the Boost version, and then type

    makedepend
    make

