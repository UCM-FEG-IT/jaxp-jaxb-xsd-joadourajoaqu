# XSD-JAXP-JAXB

## Cloning a Git Repository

To get a copy of an already existing Git repository, you need to clone it. Make sure you know the Git repository URL before starting the Clone Repository wizard in the IDE.

1.  Choose Team > Git > Clone from the main menu. The Clone Repository wizard displays.
    
    [![Clone Repository wizard](https://netbeans.org/images_www/articles/74/ide/git/clone-wizard-small.png)](https://netbeans.org/images_www/articles/74/ide/git/clone-wizard.png "Clone Repository wizard")
    
2.  At the Repository page, specify the path to a Git repository location, user name and password (you can save them for the future if required).
3.  (Optional) Click Proxy Configuration to display the Options dialog box and set the proxy server settings. Click OK when finished.
4.  Click Next to switch to the next step of the wizard.
5.  At the Remote Branches page, select the repository branch(es) to be fetched (downloaded) to your local repository. Click Next.
6.  At the Destination Directory page, specify the following:
    -   In the Parent Directory field, the path to the directory intended for the cloned repository on your hard drive (alternatively, click the Browse button and navigate to the directory).  
        The Parent Directory field is pre-filled with the path to the default NetBeansProjects directory where all NetBeans projects are stored.
    -   In the Clone Name field, the name of the local folder where the original project will be cloned to.  
        By default Clone Name is filled out with the actual Git repository name.
    -   In the Checkout Branch field, select the branch to be checked out into the working tree.
    -   In the Remote Name field, the name that represents the original repository being cloned.  
        origin is the default alias of the repository being cloned. It is a recommended value.
    -   Leave the Scan for NetBeans Projects after Clone checkbox selected to activate after-scanning right after the clone finishes. (The plugin searches for NetBeans projects in the cloned resources and offers to open the found projects.)
7.  Click Finish.  
    After a Git repository is cloned, the metadata .git folder is created inside the folder you selected in the wizard.

## Committing Sources to a Repository

To commit files to the Git repository:

1.  In the Projects window, right-click the file(s) you want to commit.
2.  In the context menu, choose Git > Commit.
    
    The Commit dialog box displays.
    
    [![Commit dialog box](https://netbeans.org/images_www/articles/74/ide/git/commit-small.png)](https://netbeans.org/images_www/articles/74/ide/git/commit.png "Commit dialog box")
    
    The Commit dialog box contains the following components:
    
    -   Commit Message text area intended for describing the change being committed
    -   Author and Commiter drop-down lists that allow to differentiate between those who made the change and who physically committed the file if necessary.
    -   Files to Commit section that lists:
        
        -   all files modified,
        -   all files that have been deleted in the Working Tree (locally),
        -   all new files (i.e. files that do not yet exist in the Git repository),
        -   all files that you have renamed.
            
            Two toggle buttons that switch the mode in which the actual commit is to be performed are available here:
            
            UI Component
            
            Name
            
            Description
            
            ![Changes between HEAD and Index](https://netbeans.org/images_www/articles/74/ide/git/changes-head-index.png)
            
            **Changes between HEAD and Index**
            
            Displays a list of files that are staged.
            
            ![Changes between HEAD and Working Tree](https://netbeans.org/images_www/articles/74/ide/git/changes-head-wt.png)
            
            **Changes between HEAD and Working Tree**
            
            Displays a list of files that are either already staged or only modified/created and not staged yet.
            
        
        **Note**: To specify here whether to exclude individual files from the commit, either deselect the checkbox in the first column called Commit or right-click a file row in the Commit Action column and choose Exclude from commit from the pop-up menu. To display the Diff Viewer here, right-click a file row in the Commit Action column and choose Diff from the pop-up menu.
        
    -   Update Issue section intended for tracking issues related to the change being committed.
        
        **Note**: You need to install the JIRA or Subversion plugin to start tracking issues in the IDE.
        
3.  Type in a commit message in the Commit Message text area. Alternatively, you can do any of the following:
    -   click the Recent Messages ( ![Recent messages icon](https://netbeans.org/images_www/articles/74/ide/git/recent-msgs.png) ) icon located in the upper right corner to view and select from a list of messages that you have previously used,
    -   click the Load Template (![Select template icon](https://netbeans.org/images_www/articles/74/ide/git/msg-template.png)) icon located in the upper right corner to select a message template.
4.  After specifying actions for individual files, click Commit.  
    The IDE executes the commit and stores your snapshots to the repository. The IDE's status bar, located in the bottom right of the interface, displays as the commit action takes place. Upon a successful commit, versioning badges disappear in the Projects, Files and Favorites windows, and the color coding of committed files returns to black.

# Activity ONE - Clone this repository using NetBeans
# Activity TWO - Do The Workshops deescribed in the PDF using netbeans on your computer
# Activity Three - Commit the changes to github once you are done
