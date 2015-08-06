Repository URL:
https://github.com/PhillipKatz/Modulaser

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Intro
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Modulaser is an analytical tool, used to determine various qualities of an Object-Oriented program; specifically and most importantly: modularity

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Limitations
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Modulaser started out as a research project, hence it had to undergo several changes before becoming a user-friendly tool.
Because of it, it contains the following limitations and problems (all somewhat easy to fix, but won't be attended to, unless someone would show interest in the product as a tool):

-The program currently supports only Windows OS.
	Expected future expansion: support of Linux OS
-The tool is only capable of analyzing Java programs.
	Expected future expansion: capability to analyze C# programs

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Terms of Use
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Even though the following scenario is extremely unlikely: No responsibility shall be taken for any damage caused by this program's use or misuse, and no compensation would be given either.


"You also agree that you will not use these products for any purposes prohibited by United States law, including,
without limitation, the development, design, manufacture or production of nuclear, missiles, or chemical or biological weapons"
~ iTunes terms of service.
	Yes, you're not allowed to use iTunes for nuclear weapons. Please don't use this software for that either.

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Instructions
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Generally it should all be intuitive, so you're probably better off trying things for yourself rather than reading this section.
If anything's extremely hard to figure out in particular, please do contact me; Let me know about what needs fixing.

Downloading:
-Enter the following URL: https://github.com/PhillipKatz/Modulaser
-Click the "Download ZIP" button
-Extract the contents of the ZIP file (suggested programs for that: either "WinRAR", or "WinZip").

Running:
-Double-click the extracted "Modulaser.jar" file.
	Notice: the program writes files to the same directory this .jar file is in.

Usage:
-Initial interface:
	1) Check the boxes you want (suggestion: leave them checked), and click the button.
	2) Browse your computer: choose a folder which contains the project you want to analyze. It has to contain the compiled classes.
		Notice: Modulaser would find the files needed for analysis by itself. Just make sure your chosen folder contains them, and that it won't contain other programs you don't want to analyze.
-Graph GUI:
	-If you're just interested in the analysis, click on "Analyze" on the side-bar menu, then on "Derive Modularity Matrix".
	-Use your mouse-wheel to zoom-in/out, and drag your mouse across the graph to pan. Click elements to choose and relocate them.
	-Use the side-bar menu to manipulate the graph further.
-Modularity Matrix GUI:
	Notice: depending on whether you left the according checkbox checked at the beginning, the program may have already been analyzed for you.
	-Perform manipulations on the matrix with the various buttons now available
	-change your view of the matrix using the GUI at its corner.
	-Save the image presented in the Matrix panel, the (text) conclusions of the analysis, or the program-data itself (the state of the matrix) to files.
	
-Notice: as stated before, the output files are saved to the same directory in which the JAR file is in. All of the output files are saved in a single folder, called "saved_output"

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Ownership
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Disclaimer:
This program contains a third-party library, which is used to read compiled classes.
The mentioned library is called "ByteCode Engineering Library", and is owned by Apache organization (c)
The library can be read about and downloaded from the following address: https://commons.apache.org/proper/commons-bcel/

The rest of the program was written by Phillip Katz (contact: phillipkatz1@gmail.com), and supervised by Dr. Iaakov Exman (contact: seproject@jce.ac.il)

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Demonstration
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

For your convenience, an example-purposed item has been added.
It's an Android program: A Ping-Pong game I've made.
You'll find it at the same place you'd find the Modulaser runnable JAR file.

You may experiment/test Modulaser's functionality by analyzing it, instead of one of your own programs.
To do so, simply run "Modulaser.jar", and when you browse for a program to analyze, choose the "example" folder. If you're not sure how, read about it in the "Instructions" section.
