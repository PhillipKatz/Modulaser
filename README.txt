Repository URL:
https://github.com/PhillipKatz/Modulaser

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
1. Introduction
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Modulaser is an analytical tool, used to determine various qualities of an Object-Oriented program; specifically and most importantly: modularity

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
2. Limitations
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Modulaser started out as a research project, hence it had to undergo several changes before becoming a user-friendly tool.
Because of it, it contains the following limitations and problems (all somewhat easy to fix, but won't be attended to, unless someone would show interest in the product as a tool):

-The program currently supports only Windows OS.
	Expected future expansion: support of Linux OS
-The tool is only capable of analyzing Java programs.
	Expected future expansion: capability to analyze C# programs

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
3. Terms of Use
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Ownership:
Except for the library referred in the Disclaimer below, the whole program was designed and written
by Phillip Katz, and supervised by Dr. Iaakov Exman (for contact information, see "Technical Support").

Disclaimer:
This program contains a third-party library, which is used to read compiled classes. 
The mentioned library is called "ByteCode Engineering Library", and is owned by Apache organization (c) 
The library can be read about and downloaded from the following address: https://commons.apache.org/proper/commons-bcel/ 


Download and acquisition:
You may download this program any number of times, and hold any number of its copies.


Use of the program:
You may use the program or any of its parts.
You may redistribute the program, as long as you make a clear reference to its original creator.
You may not take credit for the program's contents, used ideas and design, nor claim to have any other connection you don't have with it.
You are not allowed to sell or redistribute the program or its parts for personal gain.


Payment:
This program is a free and open-source software. Third-party selling of its contents are prohibited.


Warranty:
Even though the following scenario is extremely unlikely: No responsibility shall be taken for any damage caused by this program's use or misuse, and no compensation would be given either.

Technical Support:
Program writer: 	Phillip Katz 		(contact: phillipkatz1@gmail.com)
Supervisor:			Dr. Iaakov Exman	(contact: iaakov@jce.ac.il).

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
4. Instructions
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Downloading:
-Enter the following URL: https://github.com/PhillipKatz/Modulaser
-Click the "Download ZIP" button
-Extract the contents of the ZIP file (suggested programs: either "WinRAR", or "WinZip").


Running:
-Double-click the extracted "Modulaser.jar" file.
	Notice: the program writes files to the same directory this .jar file is in.


Usage:

-Initial interface (titled "Prog. Chooser"):
	1) Check the boxes you want (suggestion: leave them checked), and click the button.
		Note: if you're not sure what the checkboxes do, hover your mouse over them to get an explanation.
	2) Browse your computer: choose a folder which contains the project you want to analyze. It (only) has to contain the compiled classes of the analyzed folder.
		Notice: Modulaser would find the files needed for analysis by itself. Just make sure your chosen folder contains them, and that it won't contain other programs you don't want to analyze.

-Graph GUI (titled with the name of analyzed program, or its folder name):
	-If you're just interested in the analysis, click on "Analyze" on the side-bar menu, then on "Derive Modularity Matrix".
	-Use your mouse-wheel to zoom-in/out, and drag your mouse across the graph to pan.
	-Click elements to choose and relocate them.
	-Place your mouse over an element to read its name (element name tags are otherwise readable only at certain magnification)
	-Use the side-bar menu to manipulate the graph further.
	Side bar:
		View pane: viewing options. Includes zooming and panning. Useful if your mouse-wheel doesn't work for some reason.
		Observe pane: change observation of graph. Includes the marking of different-typed components (which also unlocks them, allowing thei relocation), and show/hide graph edges.
		Arrange Graph pane: various options for automatic re-sorting of the graph
		Analyze pane: provides analytical tools, which currently include (only) analysis through the use of a modularity matrix.

-Modularity Matrix GUI:
	Matrix visual GUI (titled "Present Modularity Matrix"):
		The modularity matrix displays links between structures (upper row) and functions (left column). The modularity of the analyzed program is determined by the linear dependency of the matrix's rows / columns.
		Several components may be grouped as a single structure or functional element; in which case they're written together, with commas used for separation. "<init>" functions represent constructors.
		The structure/function names may get cut-off, as their writing space is limited.
		-"set column start" / "set row start" buttons: determine from which index first column / row shall be drawn.
		-"set columns displayed" / "set rows displayed" buttons: determine how many columns / rows are drawn.
		-arrows: view next group of columns / rows in matrix
		-matrix cells: may be clicked to create or remove links
	Buttons GUI (titled "Modularity Matrix Controls"):
		includes various buttons, past saves (if any save has been made), and basic matrix info. If the matrix hasn't been organized yet, the program would suggest what button you should press by highlighting it in red.
		-"generate modularity matrix" button: re-draws the matrix
		-"enable large matrix draw" button: changes the drawing of the matrix; the matrix is drawn in its entirety, without navigation tools (may fail if matrix size exceeds screen size).
		-"change links manually" button: enables toggling links through mouse-interaction with the matrix
		-"Automatic Reduction" button: eliminate blank and duplicate rows/columns
		-"Automatic Diagonalizing" button: automatically sort the matrix to a block-diagonal matrix.
		-"Group links to blocks" button: register bundled "blocks" as unified groups.
		-"Mark diagonal blocks" button: color the blocks to distinguish between modular and non-modular blocks.
		-"remove empty rows" / "remove empty columns" buttons: removes blank rows/columns from the matrix
		-"unite identical rows" / "unite identical columns" buttons: groups identical functions/structures as one function/structure.
		-"swap rows" / "swap columns" buttons: enables the swapping of rows and columns through mouse-clicks performed on the matrix.
		-"shift positions" button: allows moving a cell in the matrix through mouse-clicks performed on the matrix. The movement does not disturb the matrix's main diagonal (if said diagonal has already been sorted).
		-"save conclusions" button: generate a text file with insights gathered through the modularity-matrix.
		-"save image" button: capture and save the matrix's current display to an image (".png") file.
		-"save matrix" button: save current matrix state into a file; the save can be loaded anytime, even after program close (process takes ridiculously long time, and has been disabled until further notice).
		-"load pre-existing matrix" button: load a save file that has been generated in a previous session.
		-"load matrix" buttons: appear only when at least one save has been made in current session. Lets the user return to a previous state.
		
	Notice: depending on whether you left the according checkbox checked at the beginning, the program may have already been analyzed for you.
	-Perform manipulations on the matrix with the various buttons now available
	-change your view of the matrix using the GUI at its corner.
	-Save the image presented in the Matrix panel, the (text) conclusions of the analysis, or the program-data itself (the state of the matrix) to files.
	
-Notice: as stated before, the output files are saved to the same directory in which the JAR file is in. All of the output files are saved in a single folder, called "saved_output"


------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
5. Demonstration
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

For your convenience, a sample program has been added.
It's an Android program: A Ping-Pong game I've made.
You'll find it at the same place you'd find the Modulaser runnable JAR file.

You may experiment/test Modulaser's functionality by analyzing it, instead of one of your own programs. If needed, follow these instructions (an explanation about the GUI itself can be found in section "4. Instructions")
If any of the following steps fail, you may contact support (refer to contact information in "3. Terms of Use" -> "Technical Support")
1) Run "Modulaser.jar", and when you browse for a program to analyze, choose the "example" folder. If you're not sure how, read about it in the "Instructions" section.
2) Uncheck the box that says "Automate Analysis Choices" 
3) Click "analyze program of choice"
4) Browse your computer for the folder which contains the program you wish to analyze. The folder you choose must contain (directly or through subfolders) the analyzed program's compiled classes.
 
If the program was loaded correctly you'll be presented with a panel which holds a graph and a side-bar.
If you left the "Automate Analysis Choice" box checked, the program would do the rest of the analysis by itself, present the final matrix, and save its result to Modulaser.jar 's directory, in a folder called "saved_output".
In case the "Automate Analysis Choice" box was left unchecked:
	5) Click "Analyze" in the sidebar, and then click "Derive Modularity Matrix". This should launch 2 new panels: the modularity matrix's controls, and its presentation.
	6) Click on "generate modularity matrix"
	7) The program would instruct you to press 4 buttons at a certain order: Click the red-marked buttons to organize the matrix into block-diagonal form. 
	8) The matrix would reach a form in which all of its links (active cells) are organized as a diagonal that's made out of squares.
	9) Click on "save conclusions", also "save image" if you'd like.
	10)View the output results in the generated save-folder (mentioned after step 4)
