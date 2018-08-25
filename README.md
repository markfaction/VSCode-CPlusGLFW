# C++ GLFW Development Workspace for Visual Studio Code

This repository is a VS Code workspace template for a simple C++ application that uses the [GLFW library](https://www.glfw.org/). For anyone preferring a lightweight editor to develop C++ OpenGL graphics/games applications using the GLFW library (under Windows OS), this VS Code workspace is a basic starting point. The workspace and configuration can be extended and modified in any way required for practical projects and applications.

### Prerequisites
- Its assumed you already have an installed instance of VS Code up and running
- You have MinGW installed in your machine
- The 'Windows pre-compiled binaries' are downloaded from the [GLFW downloads page](https://www.glfw.org/download.html) (The file I downloaded was glfw-3.2.1.bin.WIN32.zip. Yours may be different depending on newer releases of GLFW)
- Extracting the file downloaded from above step, the GLFW folder found inside the include folder should be copied to 'MinGW\include' in your local machine (i.e. in my case I copied the contents of **glfw-3.2.1.bin.WIN32\include** into **C:\MinGW\include**)
- Similarly, the libglfw3.a and libglfw3dll.a files inside the lib-mingw folder should be copied into the 'MinGW\lib' folder in your local machine (in my case, copying **glfw-3.2.1.bin.WIN32\lib-mingw** contents into **C:\MinGW\lib**)

### Using the VS Code Workspace
- Clone the repository or download the repository contents to your local machine
- Open the root folder (the folder which contains the **.vscode** folder) in VS Code
- Click on **View -> Integrated Terminal** to open up the integrated terminal
- Click on **Tasks -> Run Tasks**, and you should be prompted with a task named 'Build Application Task'. This is a task specified in the tasks.json file that runs a simple batch file (build.bat) which does the compiling and linking steps, and runs the generated executable binary (app.exe).
- Run the task 'Build Application Task'. You should see some output in the integrated terminal, and the application should execute presenting a window created by GLFW.
- (Optional) Click on **File -> Preferences -> Keyboard Shorcuts** and add a custom shortcut to running the task

### Finally...
- Extend the code & build process, add more libraries, and enjoy building that next OpenGL graphics application or game! :) 




