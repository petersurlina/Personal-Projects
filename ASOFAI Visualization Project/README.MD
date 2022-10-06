# A Song of Fire and Ice Character Relationship Visualization
---

[View Notebook](https://github.com/petersurlina/Personal-Projects/blob/c62726c86cb2eab8360dcc6cf0b1ccf67c470097/ASOFAI%20Visualization%20Project/Project_Files/A%20Song%20of%20Fire%20and%20Ice%20Character%20Analysis.ipynb)

## Project Objective

The main objective of the project notebook is to visualize the most mentioned realtionships in the "A Song of Ice and Fire" book series. People may know this book series better by its TV adaptation, "Game of Thrones". However, the books have thousands of various characters appear throughtout its writing. The database I used for this project was not my own, it is actually available  on Kaggle.com. (Link: https://www.kaggle.com/datasets/marinl/assignement-1-got) Now I know this dataset is not complete since in total it has 2,824 relationships identified even though the total character count in the books come out to roughly 2,102 characters. Relationships on their own would be tens of thousands, if not hundreds of thousands, of differing entries. To obtain this data I imagine the original poster wrote a program that would scan the text of the books using some sort of [Natural Language Processing model](https://www.ibm.com/cloud/learn/natural-language-processing). From there they could develop these relationships as they appear in the text and the weight count would be adjusted based on the number of interactions the characters have throughout the series.


## Recreating the project's environment

#### *This setup is for Windows Environments running Python

This project also assumes you have a general knowledge of local directory management and can follow along with the setup even if you have different names for files.

1. Install Python (https://www.python.org/downloads/)
2. Install Pycharm IDE (https://www.jetbrains.com/help/pycharm/installation-guide.html)
3. Create a desktop folder to store the project (* I used a folder called replica_project)
4. Run Pycharm

- Create new Project using venv (Virtual Enviornment) in Pycharm 

![Python Setup](https://user-images.githubusercontent.com/54562962/194196957-699c2bcb-b441-4a57-a4ad-37a594b8faf3.jpg)

- Once inside the IDE navigate towards the bottom of the screen and open the terminal tab
- Ensure you are set in your project directory

![Terminal](https://user-images.githubusercontent.com/54562962/194197575-6bc51bc0-e039-4dd0-96e4-79f462629426.jpg)

 ### Run the following Commands
```
pip install --upgrade pip
```
if ERROR: Could not install packages due to an OSError: [WinError 5] Access is denied: 'C:PATH' Check the permissions.
(See https://www.youtube.com/watch?v=rKYRcwbFp6Y&ab_channel=StudySession for solution)
- Make sure to save change made to pyvenv.cfg file and continue running commands
```
python -m pip install jupyter
pip install pandas, networkx, pyvis, matplot, scipy, python_louvain
```
5. Add Scripts path from inside project Folder to PATH settings
- Navigate to your project folder

![Path1](https://user-images.githubusercontent.com/54562962/194244524-a5650cfe-ed90-4144-a62b-97da3b92b108.jpg)

- Go into the "venv" folder
			
![Path2](https://user-images.githubusercontent.com/54562962/194244582-4b745633-65bc-49b4-94ec-32eccadb695f.jpg)

- Go into the "Scripts" folder

![Path3](https://user-images.githubusercontent.com/54562962/194244646-d9745762-5db9-497a-ba59-bd66cfa80170.jpg)

- Copy the path of the scripts folder by right clicking in the white space of the overhead directory bar
- Search "PATH" in the windows bar -> Click on the "Edit system environment variables" option
- Click the "Environment Variables..." button
 
![insert1](https://user-images.githubusercontent.com/54562962/194244833-c6543d56-1144-489c-b0ab-7bda30db1d4e.jpg)

- Under the second window labeled "System Variables" scroll to "Path" and open it

![insert2](https://user-images.githubusercontent.com/54562962/194244997-762c0266-d28e-4860-9b69-af8de2070148.jpg)


- Finally, click the new button and copy the path to scripts (ctrl + v to paste)

![insert3](https://user-images.githubusercontent.com/54562962/194245061-89216a00-ecd8-48ee-b558-5c56331c67c3.jpg)

* Make sure to OK through all three windows open to save this adjustment

6. Restart the Pycharm IDE and go back into the terminal interface
- Run the following commands:

```
python -m jupyterlab build	*May take a few minutes to create 
python -m jupyterlab		(Builds pipeline on local directory and should open in a new browser tab)
```

- Now exit the JuypterLab browsing tab and go into Pycharms IDE Terminal
- Press "ctrl + c" twice to break the pipeline
- Copy the contents of Project_Files into Project Folder

![Added](https://user-images.githubusercontent.com/54562962/194246336-bc3e985b-884e-44f7-a420-a29bff8f07d6.jpg)

Rerun the following command in Pycharms IDE terminal window (Confirm new files show up on left hand side of notebook):
```
python -m jupyterlab 
```

![new_files](https://user-images.githubusercontent.com/54562962/194246608-98ff4aae-01b0-4dfe-9e02-b9e45ba1871c.jpg)

- Once inside Jupyter Lab double click "A Song of Fire and Ice.ipynb" in order to access the notebook
- Press (Restart the Kernel + Run > Run All Cells) To view all graphs and data inside the notebook
 
From this point on you are free to manipulate and view the graph visualizations that do not appear in this GitHub repository.

## Personal Motivation
My whole reason for creating this project was to learn more about data visualizations and what technologies were available for me to do so. I decided on utilizing Jupyter Lab after doing some quick reading on available free technologies. I wanted to test the usability of Jupyter Lab's notebook style so I took the leap and ultimately was pleased with the results.

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
