# CSV_Tool-Releases
this is where the installer for the tool and the tools executables and binaries are. Using the installer is the required way to download the tool and any other way would be unsupported
## 🛠️ Using The Installer
1. to download the installer on windows follow steps 2 through 6 then skip to step 10 if you are installing on Debian Linux skip to step 9
2. from the repository on your web browser click on the `WindowsInstallerForCSVTOOL&RDTOOL.exe` file to open it
3. On the file preview screen, locate the group of 3 buttons in the top-right corner (the first button is labeled **Raw**).
4. Click the 3rd button on the right (the download icon, which shows the tooltip **"Download raw file"** when you hover over it) to save the file to your computer.
5. it does not matter what folder you save the installer in however you should note where it is as you will need it in the next step if on linux skip step 6
6. to run the installer on windows left click the installer file and in the following menu hit the run as administrator and when prompted click the yes button now skip to step 10 of these instructions
7. to run the installer on linux you need to give it execution permissions if not familiar with giving those permissions please search google on how to give a program execution permissions
8. once it has permissions simply double click the file and if prompted select run skip step 9 as you should have already followed it
9. for linux installing the instructions are the same as steps 2 through 6 except the name of the file is `InstallerForCSVTOOL&RDTOOLLinuxBinary` once 2-6 have been followed with that in mind do steps 7 and 8 then skip to step 10
10. once the installer window is open choose custom or standard installation standard is for non-technical users while custom is for technical users and users who want to determine what versions and folders the tools install themselves in
11. hit the next button once you have made your selection and then if you have selected custom install make the necessary selections and hit next again
12. there is one more screen which has options in both modes these options are for users who want to use a different template file than the one that's out of the box on windows there is an option for desktop shortcuts see the below notes if you are choosing to use a different template file or if you are on linux
> **Note:**  If you choose not to use the default templateFile.csv you will need to make your own one line file with the same file name that has all of your desired headers
> **Note:** for Linux users the folder that the tools install themselves in is the user's home folder in a subfolder named CSVTOOL this is important because the tool will not make desktop shorcuts
11. once you make your decisions as far as these options are concerned hit the next button
12. on the next screen  when ready hit the install now button and wait for the progress bar to finish if on linux see the below note
> **Note:** on linux the installer will give you a command to copy for giving the 2 tools execution permissions so remember to type sudo and a space before pasting the command when prompted enter your sudo password
## 💻 Using The Raw Data Tool
1. double click the Desktop shortcut the installer created if on windows on linux you would find the folder of the tool and double click the binary file (if prompted select run)
2. click the <kbd>Add Files...</kbd> button near the top of the window and next to the white box labeled Input Headless Files then select your files for the current year using windows file explorer
> ‼️**IMPORTANT NOTE** ‼️ **DO NOT** change the location of the temp file in the input window the only reason it is there is so that if we were to later need other use cases they may want to change that but as long as you are dealing with carbon data you **SHOULD** ***NEVER*** touch that input
3. once you've added all the data files for this particular year please remember to name the output file after the year
4. then select either Chronological or Reverse Chronological depending on what you need but please use same order for all your files 
> **Note:** the default is Chronological if unsure use that
5. once you are done naming the output file click the <kbd>Merge & Apply Headers</kbd> button
6. press the <kbd>Okay</kbd> button on the success prompt and check the folder where your output is for a headered file with dates ordered by whatever you selected in step 4
> **Note:** now this file is ready for the next tool
7. to create the next file hit the <kbd>Clear All</kbd> button (located below the <kbd>Remove Selected</kbd> button and next to the white box that displays your file inputs)
8. Now repeat steps 2 through 7 until all headered year files have been properly generated
## 💻 Using The CSV Tool
### 1. Selecting The Input and Output Files
1. First you will need to double-click the desktop shortcut
2. Next you will need to hit the <kbd>Browse...</kbd> button in the program window next to the `input file:` label and after the white input box
3. Navigate to your data file's location using windows file explorer and select the file
4. If you want to use multiple files here hit the <kbd>+ Add Input File</kbd> button at the bottom of the file options box until you have enough input file items (if you hit this button too many times just use the <kbd>Remove</kbd> button (it's the last button) on any file inputs that are not needed) then repeat steps 2 and 3 until all input files have been selected
> **Optional Step 5:** the output file will automatically name itself after your input file's name with `_processed.csv` on original file name (it uses the first file name) if you do not want the output file to be named this way please click the <kbd>Browse...</kbd> button on the end of the input labeled output file and navigate to the place you would like to have your output file then name it whatever you want
### 2. Selecting The Fields
1. There are 2 ways to input fields if you have a preset file skip to step 4 if not go through steps 2 and 3 and skip step 4
2. use the searchable drop down menu to select your fields
3. once you select the fields using the searchable drop down you can rename them in the output column renaming menu
4. if you have a 2 line preset file load it in the input labeled Header Preset File (2-line): by clicking the <kbd>Apply Preset File</kbd> button and then using file explorer to navigate to your preset csv file and select it the tool will auto-load the fields in your preset and rename them according to what you have set in the second line of your preset file
### 3. Selecting the Dates
1. please enter a comma separated list of start dates into the field named Start Dates and then a respective list of end dates into the field labeled End Dates please make sure you follow the requirements below when entering dates
> **Important Requirements:** It is important that you make sure to enter an equal amount of start and end dates. it is important you follow the format that the program asks for as anything not in this format will generate malformed files and possibly require manual clean up (see troubleshooting for what to do if this does happen). Also remember any dates not present in your data files should not be used so make sure you know the date ranges of your files before searching(see troubleshooting if this happens).
2. once you have correctly entered the dates hit the <kbd>Start Processing</kbd> button on the bottom left of the window next to the <kbd>Show Debug Window</kbd> button.
> **Note:** the Show debug window button is only for finding problems with the application and you should not need it
### 4. Checking The Output File
1. after the processing is finished there should be a pop up saying the processing completed successfully click the <kbd>okay</kbd> button
2. now open the output file with whatever program you wish and check that your filtered data is there
> **Note:** if you kept the default it will have made the output in the input file folder with the same name as the first input file (without the .csv) plus `_processed.csv` on the end of it
## 🪛 trouble shooting:
1. if you have accidentally entered in correct date formats or if you entered incorrect dates and generated malformed output please search where you put your output file for what you named it and delete any files you find
2. go back to the tool and correct your input and try again
