# Version Control: 
is a system that allows us to revisit our various versions of our work, it also allow us to go back and forth between our versions and track our modifications easily and compare our changes.
one of the great advantages of VCS that it allow us to recognize the mistakes easily.
## types of Version Control:
1. **Local Version Control:** it has been used by programmers many years ago it works by having one database on the computer hard drive to store changes.
2. **Centralized Version Control:**
Unlike the LVC there is no need to store database in your hard drive but your computer will be connected to a server and this server will store all the changes and files.
*Benefits of CVC:*
* Allowing the team to know who is working on what.
* Giving the administration more Control.
3. **Distributed Version Control:** it allows clients to create mirrored repositories these data backup can easily be placed on server to replace any lost data.
*Benefits of DVC:*
* It prevents the issues that happen on CVC and LVC
* Team members can work together in various ways to complete a joint projects.

## Git Features:
1. **Snapshots**: Git uses DVCS to store data in a file by using commit comand it take snapshot of your work and creates a new version of it.
2. **Local Operation**: Git relies on local Operation because most of neccessary information in local resource. *Benefits of Local Operation*:it eliminates the needs to fitch history info from server even if not connected to the internet.
3. **Tracking Changes** : Git allows you to keep track of changes because every change stored.
4. **Loss of data**: The possibility of having loss of data is significantly minimized.

5.** States** : Three main states in  git files:

1. Commited: Data is securly stored in local database.
2. Modified: Files can be changed but not commited to the database.
3. Staged: Files changed version to be commited in the next snapshot includes.
## Graphical Client:
Git includes it own GUI but it allow the programmer to use third party tool.

## Seeing your Remote: 
it helps us to view short names for all the remote URL.

 To create a new remote you can use : *command git remote add shortname url*

To fitch a remote: *git fetch [remote-name]*.

To push a remote: *git push [remote-name][branch-name]*.

To rename a remote:*git remote rename js jane*

To remove a remote: *git remote rm jane*



