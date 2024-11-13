# cintel-04-local

## Mee Vang
## P4: Publish Interactive Reactive App & Engage

Objectives
This project will much more closely follow the typical workflow of a real interactive development project. In Module 4, we create a repo in GitHub, clone it down, create a local project virtual environment in the .venv folder, activate our .venv virtual environment, and install all the packages we need.

Once the project virtual environment has everything required, we can open the project folder in VS Code, open a terminal, activate the project virtual environment (so we have access to the packages we installed into .venv), and run our app. We edit and rerun as often as needed - remember to activate your project virtual environment each time you work on the project. 

Example Project
The example project has the detailed set of steps and example code: 

https://github.com/denisecase/pyshiny-penguins-dashboard-expressLinks to an external site.


Prerequisites
To ensure a smooth experience, confirm the following are in place:

Python installed and in your path. 
Git installed and configured with user.name and user.email that matches GitHub.
VS Code installed with the Python extension. 
A GitHub repository named cintel-04-local with 4 useful files named: .gitignore, README.md, requirements.txt, app.py.
The recommended process will transfer the project to our local machine for development. Although it involves many steps, it's a procedure you'll repeat often during your degree and in your work as a data analyst. By the time you graduate, it will be second nature. Bring your courage and a sense of humor - there's no simple way to do this, so let's get started. 

The full process is also presented in the README.md of the example project: https://github.com/denisecase/pyshiny-penguins-dashboard-expressLinks to an external site.

Action 1. Open VS Code
Launch VS Code from your Start Menu, Desktop, or Taskbar.

Action 2. Open a Terminal in VS Code
Within VS Code, access the terminal by navigating to View > Terminal or Terminal > New Terminal from the menu. Alternatively, you can use the shortcut `Ctrl + ``` (the backtick key) to open the terminal pane.

The terminal type should be PowerShell for Windows, zsh (the default) for Mac, bash or similar for Linux. 

For Mac/Linux users, proceed with the default terminal. For Windows users, if cmd is the default terminal type, switch to PowerShell. Here's how:

With a terminal open, click on the dropdown arrow next to the "+" icon in the terminal pane. It's the upper right of the terminal area. 
Select Select Default Profile.
Choose PowerShell from the list. This changes the default terminal type to PowerShell. From now on when you open a terminal, it will be PowerShell. PowerShell is the more modern terminal. These commands have been thoroughly tested to work in PowerShell.  
Action 3. Clone the GitHub Repository
Navigate to the GitHub repository in your web browser and copy the repository URL.

Back in the VS Code terminal, navigate to your Documents folder before cloning the repository. Follow these steps to ensure you are in the right directory. 

Windows users:

cd ~\Documents
Mac/Linux users

cd ~/Documents
Then, clone the GitHub repository down to your machine by replacing url with the actual GitHub project repository URL you copied, and press Enter. 

git clone url
 

We recommend you choose the Documents folder as the location for all your Git repositories. 

Important: Never use spaces in folder names or file names when working with code. It will complicate your life and is generally NOT worth it. 

Action 4. Access the Cloned Repository in VS Code
After cloning, if it asks you to open this as a workspace or something, say Yes.

The repository folder is now available on your local machine and in VS Code.

We recommend you work on exactly one project repository folder at a time in a VS Code window. Always work with the whole project folder, and only one project folder at a time.

If you come back to work on this project later, you can use the File menu in VS Code to select "Open Folder", and choose the cloned repository folder. 

Action 5: View/Edit Files
Click on any file in the VS Code explorer window to view or edit it. The files you'll find include:

README.md
.gitignore
app.py
requirements.txt
 

Action 6: Create Virtual Environment (one-time)
In a VS Code terminal in the root project folder (cintel-04-local):

Run `py -m venv .venv` to create a virtual environment in the directory named .venv.   Mac/Linux may need python3 instead. Get the spacing and folder name (.venv) exactly correct. 

py -m venv .venv
Be patient, it may take a while. Post your name and Action 6 screenshot while you wait. 

Action 7: Verify .gitignore includes .venv/
In VS Code, open your .gitignore file. Verify it includes an entry for .venv/ - we do NOT want all the contents of our project .venv to go in our repo. It's not our work and we use it, but we never work directly in the .venv folder. Note: Other instructions may name this folder venv instead of .venv.  We only provide support when you use the commands as provided. If you can manage your virtual environment successfully in a different way, you are free to do so. If you experience problems, follow the exact commands and process provided. (There are infinite variations in Python - it is not feasible or useful to support them all.) 

Action 8: Activate the Virtual Environment (often)
In a VS Code terminal in the root project folder (cintel-04-local). 

We're running a script that was installed into our project virtual environment .venv folder - you can take a quick look in there to see the provided scripts. Your command is running one of the scripts installed. (Don't make any changes in the .venv folder - always work from the root project folder, but you can - and probably should - look around a bit in .venv to help understand how it is used.) 

For Windows, run `.venv\Scripts\Activate` or `.venv\Scripts\activate` in the terminal. For macOS/Linux, run source `.venv/bin/activate`.

.venv\Scripts\Activate
.venv\Scripts\activate
or

source `.venv/bin/activate`
Typically, the name of the virtual environment will appear in your terminal prompt. 

Action 9: Install Dependencies  (as needed)
Important: Verify the virtual environment is activated in your terminal before installing:

In a VS Code terminal in the root project folder (cintel-04-local) - with .venv activated:


Run pip install -r requirements.txt to install the required Python packages listed in requirements.txt. It's good practice to ensure some key packages like pip are upgraded to the most recent version before continuing. If you see a recommendation to upgrade, it's generally best to do so. 

py -m pip install --upgrade pip setuptools

py -m pip install --upgrade -r requirements.txt