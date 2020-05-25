# all-about-git
All git related learning is added as markdown files for this project.

# Git Basics:
- A version control system also called as:
    - Version Control System (VCS)
    - Source Code Management (SCM)
- Keeps track of the changes made for the code and provide a version number to every change made.
- Features:
    - Distributed version control system
    - open-source
    - free, faster
    - compatible with windows, linux, mac
    - better safeguards against data corruption
## Distributed version control
- Earlier version controls use a central repository or folder to keep tract of all the changes done to source code.
- In distributed version control, there is no central repository, Different users have different repository.
- Changes are stored as change sets instead of file changes or folder changes.
- Change sets are exchanged between repositories. Merging of those change sets or applying patches will get you the most recent code.
- No single master repository and many working copies.
- No need to communicate with a central server, Faster, No network access required while working on changes.
- No single point of failure.
- More developer interaction through forking, Developers can work independently.
- Change set submission, inclusion, rejection will be more easy.

## Installing Git
### On Windows
- Download git from [Git-SCM](https://git-scm.com/downloads)
- Double click on the installer and, install it with the defaults.
- to check if git is installed go to command prompt and run ``` git --version  ```
- If the installation was successful git will give you the version number.

## Git configurations
- Has 3 configurations System, User, Project

### System Configuration
Description | **Linux** | **Windows**
-------------------------------------------------- | --------------------------------------------- | ---------------------------------------
Configuration file Location | /etc/gitconfig | Program Files\Git\etc\gitconfig |
Command to update config | git config --system | git config --system  |

### User Configuration
Description | **Linux** | **Windows**
-------------------------------------------------- | --------------------------------------------- | ---------------------------------------
Configuration file Location | ~/gitconfig | $HOME\gitconfig 
Command to update config | git config --global | git config --global  |

### Project Configuration
Description | **Linux** | **Windows**
-------------------------------------------------- | --------------------------------------------- | ---------------------------------------
Configuration file Location | Project-Name/.git/config | Project-Name/.git/config
Command to update config | git config | git config

### general configurations to set
- Username can be set with ``` git config --global user.name "your-user-name" ```
- Email ``` git config --global user.email "your-email-address" ```
- Core editor ``` git config --global core.editor "notepad.exe --wait" ``` //will set the default editor to edit as notepad
- To read this configurations ``` git config --list ```
- Colour ui ``` git config --global colour.ui true ``` // by default this will be true

> To exit out of list use shift+q or Ctrl+q and C to exit out of running task




