#Intro to Version Control System and GIT

**VCS**:

**=>** is a system that allows you to revisit various versions of a file or set of files by recording changes. One can revert a file or project to a previous version through version control

**=>** is a system that allows you to revisit various versions of a file or set of files by recording changes. Through version control, one can revert a file or project to a previous version.

There are three types of VCS:

1. **Local Version Control(LVCS)**:  Many years ago, programmers created Local Version Control systems. A Local VCS entails one database on your hard disk that stores changes to files.

2. **Centralized Version Control(CVCS)**:  This system entails a single server storing all changes and file versions, which can be accessed by various clients. This method facilitates the collaboration between the teams of developers on a single file or set of files

3. **Distributed Version Control(DVCS)**:  addresses the major vulnerability of the CVS: the server as a single point of failure. If a CVS goes down, collaborators cannot work with each other on a file or save changes and new versions.
To prevent this type of catastrophic loss, a DVCS allows clients to create mirrored repositories. These data backups can be easily be placed on the server to replace any lost information. 

`-----------------------------------------------`

Once we explain what is VCS we can explain what is GIT

**GIT:**  Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

**Files States**: Files in Git can reside in three main states: committed, modified, and staged.

1. **Committed**: Data is safely stored in a local database.
2. **Modified**: The file has been changed but not committed to the database.

Once we explane what is VCS we can explane what is GIT

**GIT:**  Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

**Files States**: Files in Git can reside in three main states: committed, modified and staged.

1. **Committed**: Data is safely stored in a local database.
2. **Modified**: File has been changed but not committed to the database.
3. **Staged**:  Flagged a file’s changed version to be committed in the next snapshot

- **Download Git**

  Git can be installed in three ways:
   1. Install as a package
   2. Install via another installer
   3. Download and compile the source code.

  - **Mac OS X**:
    - **Terminal**: on a Mac (for Mavericks 10.9 and above) 
                    is running Git from the Terminal. If Git is not installed, you will see a prompt for installation.
    - **Git Website**: You can also download Git by visiting this                      link and following the posted directions =>                     http://git-scm.com/download/mac
    - **GitHub**: install Git as part of the GitHub for Mac install               => http://mac.github.com

  - **Windows**: 
    - **Git Website**: http://git-scm.com/download/win
    - **GitHub** : install Git as part of the GitHub
                   => http://windows.github.com
  
  - **Linux**
    - **Package Manager**:  
          You can try installing Git via your distribution’s inherent package management tool.
          You can try installing Git via your              distribution’s inherent package management tool.
        - For ***Fedora***: ```$ sudo yum install git```
        -  For ***Ubuntu***: ```$ sudo apt-get install git```

    - **Git Website**: 
        **=>** http://git-scm.com/download/linux

    

