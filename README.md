

# About The Template

This is a Microsoft Visual Studio solution template for C++ with a single project inside it.

It follows the following tutorial from <a href="https://www.youtube.com/@TheCherno">The Cherno</a>: https://www.youtube.com/watch?v=qeH9Xv_90KM



# Steps

1- Create an empty project on Microsoft Visual Studio (Uncheck the "Place solution and project in the same directory" checkbox) 
2- Click "Show All Files" button on the Solution Explorer tab to unsee all filters and see the actual project files and folders.
3- Create a folder in the main project's directory and name it "src".
4- Create a Main.cpp file in src folder.
5- Click on the main project, click properties, select "All configurations" and "All platforms" from the top.
6- Change these two settings to these:
| Option  | Will Be Changed To  |
| ------------- | ------------- |
| Output Directory  | `$(SolutionDir)bin\$(Platform)\$(Configuration)\`  |
| Intermediate Directory  | `$(SolutionDir)bin\intermediates\$(Platform)\$(Configuration)\`  |

Click apply and OK.

7- Right click on your project, do a "clean" and then "build" it.
8- You're done. Additionally if your folder (solution) has additional "DEBUG" folders you can just delete them because they were created during our steps by the old project structure.



# Things to Keep in Mind

1- Filters are nothing but "abstract folders", they don't do shit and make Microsoft Visual Studio pile up all your files in one folder making it extremely messy.
2- A solution can have multiple projects inside it, but this template only has one project inside it.



# Licensing

This template is licensed under the terms of the Apache-2.0 license. You can use this template to do whatever you want, commercially or non-commercially. Giving credits to this repository would be nice, but it is not required.

