# A Song of Fire and Ice Character Relationship Visualization
---

## Project Objective






## Recreating the project's environment

#### *This Setup is for Windows Environments running Python

This project also assumes you have a general knowledge of local directory management and can follow along with the setup even if you have different names for files.

-install Python (https://www.python.org/downloads/)
-install Pycharm IDE (https://www.jetbrains.com/help/pycharm/installation-guide.html)
	- (Optional) create a desktop folder to store the project (* I used a folder called replica_project)
	- Run Pycharm
	- Create new Project using venv (Virtual Enviornment) in Pycharm 
INSERT PICTURE -> setup
	- Once inside the IDE navigate towards the bottom of the screen and open the terminal tab
	- Ensure you are set in your project directory
INSERT PICTURE ->Terminal

	- upgrade pip	*run command: pip install --upgrade pip
		- if ERROR: Could not install packages due to an OSError: [WinError 5] Access is denied: 'C:PATH'
			Check the permissions.
			(*See https://www.youtube.com/watch?v=rKYRcwbFp6Y&ab_channel=StudySession for solution)
		- Make sure to save change made to pyvenv.cfg file

	- run command: python -m pip install jupyter
	- run command: pip install pandas, networkx, pyvis, matplot, scipy, python_louvain (Wait for confirmation of downloads)
	- Add Scripts path from inside project Folder to PATH settings
		- navigate to your project folder
INSERT PIC PATH1
			- go into the "venv" folder
INSERT PIC PATH2
			- go into the "Scripts" folder
INSERT PIC PATH3
			- copy the path of the scripts folder by right clicking in the white space of the overhead directory bar
			- now search "PATH" in the windows bar -> Click on the "Edit system environment variables" option
			- Click the "Environment Variables..." button
INSERT PIC INSERT1
			- Under the second windowed labeled "System Variables" scroll to "Path" and open it
INSERT PIC INSERT2
			- Finally, click the new button and copy the path to scripts (ctrl + v to paste)
INSERT PIC INSERT3
			- * Make sure to OK through all three windows open to save this adjustment


	- Now restart the Pycharm IDE and go back into the terminal interface
	- python -m jupyterlab build	*May take a few minutes to create 
	- python -m jupyterlab		(Builds pipeline on local directory and should open in a new browser tab)
	- Now exit the JuypterLab browsing tab and go into Pycharms IDE Terminal
	- Press "ctrl + c" twice to break the pipeline
	- Copy the contents of Project_Files into Project Folder
INSERT PIC ADDED
	- Rerun python -m jupyterlab in Pycharms IDE terminal window (Confirm new files show up on left hand side of notebook)
INSERT PIC NEW_FILES
	- Once inside Jupyter Lab double click "A Song of Fire and Ice.ipynb" in order to access the notebook
	- Press (Restart the Kernel + Run > Run All Cells) To view all graphs and data inside the notebook
 
From here you are free to manipulate and view the graph visualizations that do not appear in the GitHub repository.


## What I learned
------------------------
- Learned to implement and test data visualization libraries in python
- Got to work with a new technology, Juypter Lab
- Brushed up on knowledge of Python's List, Dictionary, and Node structures
- Learned some new sorting / querying techniques in Python
- Discovered the topics of Community detection and Centrality, as well as how and why we use them in data analysis

## Potential Changes
- [ ] Implement dynamic sizing for graphs and networks drawn
- [ ] Host the project and allow users an easier setup, rather than recreating the dev. environment
- [ ] Implement other forms of data visualizations with detailed descriptions/explanations.
