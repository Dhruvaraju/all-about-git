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
- to check if git is installed go to command prompt and run `git --version `
- If the installation was successful git will give you the version number.

## Git configurations

- Has 3 configurations System, User, Project

### System Configuration

| Description                 | **Linux**           | **Windows**                     |
| --------------------------- | ------------------- | ------------------------------- |
| Configuration file Location | /etc/gitconfig      | Program Files\Git\etc\gitconfig |
| Command to update config    | git config --system | git config --system             |

### User Configuration

| Description                 | **Linux**           | **Windows**         |
| --------------------------- | ------------------- | ------------------- |
| Configuration file Location | ~/gitconfig         | \$HOME\gitconfig    |
| Command to update config    | git config --global | git config --global |

### Project Configuration

| Description                 | **Linux**                | **Windows**              |
| --------------------------- | ------------------------ | ------------------------ |
| Configuration file Location | Project-Name/.git/config | Project-Name/.git/config |
| Command to update config    | git config               | git config               |

### general configurations to set

- Username can be set with `git config --global user.name "your-user-name"`
- Email `git config --global user.email "your-email-address"`
- Core editor `git config --global core.editor "notepad.exe"` //will set the default editor to edit as notepad
- To read this configurations `git config --list`
- Colour ui `git config --global colour.ui true` // by default this will be true

> To exit out of list use shift+q or Ctrl+q and C to exit out of running task

> Vi editor, to start editing press s, to exit out of Vi press **esc** then **:wq** and click enter

> Auto completion is a built in function for windows for mac and linux it need to be updated, the scripts for that are available in [git-autoComplete](https://github.com/git/git/tree/master/contrib/completion)

## Help in git

- use `git help` to know about the commands that can be used in git.

## Initiating a folder as git repository(repo)

- Create a folder and navigate to the folder in command prompt
- `git init` will add the folder to git version control, files ., .., .git will be generated, which will be hidden by default.
- use Dir to list those files in windows, or ls in mac or linux
- All the tracking information will be available in .git folder.

## Adding a file to git repo

- Create a new text file in the folder and save it.
- To add this file to repository you we need run the command `git add .`
  - **git add** will add the files or folders for tracking
  - **.** is to say that track all the changes made in a folder (files, folders, sub-folders .. everything).
- Once added to permanently save this changes you need to commit the changes using `git commit -m "Message for committing"`
- example `git commit -m "Initial Version"`
  > We repeat this in git, make changes => add => commit

### Convention for writing commit messages:

- Single line summary less than 50, make sure not to exceed 72 char. Clear and descriptive.
- Optionally we can add a blank line with additional description.
- Messages should be in present tense like. "Fix for the issue:2345" instead of "fixed 2345".
- User asterisks or hyphens, add tracking numbers like the example above.
- Create shorthand for the type of files delivered, or bug fix. eg: \[componentTest,CSS\], Fix#, Story#
- We can also follow git conventional commits additional information available at [conventional commits specification](https://www.conventionalcommits.org)

## Viewing commit logs

- Use command `git log` to see all the information about git commits made
- git log will give the following info

```
commit 8bf158bae06b7457b72b891b37ea73515303796b (origin/master, origin/HEAD)
Author: UserName <User-Email>
Date:   Mon May 25 11:48:17 2020 +0530

    Initial Version

// '8bf158bae06b7457b72b891b37ea73515303796b' is the unique commit number.
// 'Initial Version' is the message we added for this commit.
```

- some of the switches that can be used are:
  - Restrict number of commit logs by using `git log -n 5`
  - by time (Date in YYYY-MM-DD format)
    - git log --since=2020-05-10
    - git log --until=2020-08-10
  - by Author `git log --author="dexter"`
  - by string `git log --grep="test" ` // will get all the commits with word 'init' in commit message.

> To exit out of list use shift+q or Ctrl+q and C to exit out of running task

> Vi editor, to start editing press s, to exit out of Vi press **esc** then **:wq** and click enter

