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
- Has 3 configurations System, user, Project

System |
------------------------------------------ | -------------------------------------------------------------------------------------------
Configuration file Location | *Linux* - /etc/gitconfig, *Windows* - Program Files\Git\etc\gitconfig


