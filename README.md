[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/vbnbTt5m)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=15235595&assignment_repo_type=AssignmentRepo)
# Dev_Setup
Setup Development Environment

#Assignment: Setting Up Your Developer Environment

#Objective:
This assignment aims to familiarize you with the tools and configurations necessary to set up an efficient developer environment for software engineering projects. Completing this assignment will give you the skills required to set up a robust and productive workspace conducive to coding, debugging, version control, and collaboration.

#Tasks:

1. Select Your Operating System (OS):
   Choose an operating system that best suits your preferences and project requirements. Download and Install Windows 11. https://www.microsoft.com/software-download/windows11

   DONE WITH IT, IT WAS EASY, at some point it was hard, i used a youtube video for it

2. Install a Text Editor or Integrated Development Environment (IDE):
   Select and install a text editor or IDE suitable for your programming languages and workflow. Download and Install Visual Studio Code. https://code.visualstudio.com/Download

   I HAVE IT INSTALLED ALREADY

3. Set Up Version Control System:
   Install Git and configure it on your local machine. Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit. https://github.com
   
   SURE IT WAS EASY

4. Install Necessary Programming Languages and Runtimes:
  Instal Python from http://wwww.python.org programming language required for your project and install their respective compilers, interpreters, or runtimes. Ensure you have the necessary tools to build and execute your code.

DONE, IT WAS EASY WITH THE HELP OF THE TUTORIAL

5. Install Package Managers:
   If applicable, install package managers like pip (Python).
DONE TOO

6. Configure a Database (MySQL):
   Download and install MySQL database. https://dev.mysql.com/downloads/windows/installer/5.7.html
DONE WITH IT, THANK FOR A WELL EXPLAINED TUTORIAL

7. Set Up Development Environments and Virtualization (Optional):
   Consider using virtualization tools like Docker or virtual machines to isolate project dependencies and ensure consistent environments across different machines.

8. Explore Extensions and Plugins:
   Explore available extensions, plugins, and add-ons for your chosen text editor or IDE to enhance functionality, such as syntax highlighting, linting, code formatting, and version control integration.
    DONE THAT, I INSTALLED PRETTIER AND OTHER EXTENSION SHOWNED ON THE TUTORIAL

9. Document Your Setup:
    Create a comprehensive document outlining the steps you've taken to set up your developer environment. Include any configurations, customizations, or troubleshooting steps encountered during the process. 

Step 1: Update Windows
Go to Settings > Windows Update and check for updates. Install any pending updates and restart if necessary.

Step 2: Install Essential Tools
PowerShell: Windows 11 comes with PowerShell pre-installed.

Windows Terminal: Download from the Microsoft Store for a better command-line experience.
2. Installing Version Control
Step 1: Install Git
Download the latest version of Git from the official website.
Run the installer with default settings.
Configure Git:
sh
Copy code
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
Step 2: Generate SSH Key
sh
Copy code
ssh-keygen -t rsa -b 4096 -C "your.email@example.com"
Add the generated SSH key to your GitHub/GitLab account.

3. Setting Up Development Tools
Step 1: Install Node.js and npm
Download the LTS version from the official Node.js website.
Follow the installer instructions.

Step 2: Install Python and pip
Download the latest version of Python from the official website.
Ensure you check the box to add Python to PATH during installation.

Follow the installer instructions.
Download Maven from the official website, extract it, and add the bin directory to your PATH.
Step 4: Install Docker Desktop
Download Docker Desktop from the official Docker website.

Follow the installer instructions.
Ensure Docker Desktop is running and configure it to start on login.

4. Setting Up Integrated Development Environment (IDE)
Step 1: Install Visual Studio Code
Download from the official VS Code website.
Follow the installer instructions.

Step 3: Install Extensions
Install extensions like ESLint, Prettier, Python, Docker, etc., via the VS Code marketplace.
5. Database Setup
Step 1: Install MySQL
Download from the official MySQL website.
Follow the installer instructions.

Follow the installer instructions.
6. Configuring Shell and Terminal
Step 1: Install Windows Subsystem for Linux (WSL)
Open PowerShell as Administrator and run:
sh
Copy code
wsl --install
Restart your computer if prompted.
Set up a Linux distribution (e.g., Ubuntu) from the Microsoft Store.
Step 2: Customize Windows Terminal
Open Windows Terminal and customize settings via the settings UI.
Add profiles for PowerShell, Command Prompt, and WSL.
Step 3: Install Zsh and Oh-My-Zsh in WSL
sh
Copy code
sudo apt update
sudo apt install -y zsh
chsh -s $(which zsh)
Log out and back in for the changes to take effect.
sh
Copy code
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
7. Setting Up Virtual Environments for Python
Step 1: Install virtualenv
sh
Copy code
pip install virtualenv
Step 2: Create and Activate Virtual Environment
sh
Copy code
virtualenv venv
source venv/bin/activate
8. Setting Up Containerization and Orchestration
Step 1: Install Docker Compose
Docker Desktop includes Docker Compose by default.
Verify the installation:
sh
Copy code
docker-compose --version
Step 2: Create a Docker Compose File
Example docker-compose.yml for a simple web app:
yaml
Copy code
version: '3'
services:
  web:
    image: nginx
    ports:
      - "80:80"
9. Troubleshooting Steps
Issue 1: Permission Denied for WSL
Ensure the Linux distribution is installed correctly.
Check WSL version:
sh
Copy code
wsl --list --verbose
Upgrade to WSL 2 if not already:
sh
Copy code
wsl --set-version <distro> 2
Issue 2: Git SSH Key Not Working
Check permissions of the SSH key:
sh
Copy code
chmod 600 ~/.ssh/id_rsa
Ensure the SSH agent is running and add the key:
sh
Copy code
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa
Issue 3: Extensions Not Working in VS Code
Ensure the correct Python interpreter is selected for Python projects.
Restart VS Code after installing new extensions.
Issue 4: Node.js Version Issues
Use nvm-windows for managing multiple Node.js versions:
Download and install nvm-windows from the GitHub repository.
Use nvm to install and switch Node.js versions:
sh
Copy code
nvm install 14.17.0
nvm use 14.17.0
Issue 5: Slow MySQL Performance
Optimize MySQL configuration in my.ini.
Increase buffer pool size:
ini
Copy code
[mysqld]
innodb_buffer_pool_size = 1G
10. Additional Customizations
Step 1: Install and Configure Vim or Neovim
Install Vim from the official website or via a package manager like Chocolatey:
sh
Copy code
choco install vim
Customize ~/.vimrc or ~/.config/nvim/init.vim.


Step 3: Configure Environment Variables
Add environment variables via the System Properties > Environment Variables UI.


Verify installation and configurations:
Git: git --version
Node.js: node -v
Python: python --version
Docker: docker --version
MySQL: mysql --version
PostgreSQL: psql --version

#Deliverables:
- Document detailing the setup process with step-by-step instructions and screenshots where necessary.
- A GitHub repository containing a sample project initialized with Git and any necessary configuration files (e.g., .gitignore).
- A reflection on the challenges faced during setup and strategies employed to overcome them.

#Submission:
Submit your document and GitHub repository link through the designated platform or email to the instructor by the specified deadline.

#Evaluation Criteria:**
- Completeness and accuracy of setup documentation.
- Effectiveness of version control implementation.
- Appropriateness of tools selected for the project requirements.
- Clarity of reflection on challenges and solutions encountered.
- Adherence to submission guidelines and deadlines.

Note: Feel free to reach out for clarification or assistance with any aspect of the assignment.
