#Developer Docs#

##Cloning from GitHub##
The following assumes you are using AMPPS and Eclipse, though the steps are likely similar for other development environments. 

1. Download and extract a copy of Drupal to your AMPPS `www` folder. 
2. Rename the folder you just extracted to `famedev`. 
3. Delete the `sites` folder from `famedev`. 
4. Open Eclipse. You should be in the PHP Perspective.
5. Select `File—>Import...` and then from the dialog choose `Git—>Projects from Git`. Hit the `Next` button to continue.
6. Choose `Clone from URI` and hit `Next` to continue. 
7. Enter the URI `git@github.com:fairfield-is320-fall2014/fame.git` and select the `https` protocol. Hit the `Next` button to continue. 
8. Select the `master` branch and hit `Next`.
9. Use the browse button to set the Directory to the `famedev` folder.
10. Eclipse will automatically add `fame` to the end of the Directory. Change `fame` to `sites` instead. Hit the `Next` button to continue. Watch as it downloads all the files to the new sits folder. 
11. Select the New Project wizard. Hit the `Finish` button to continue.
12. Within the New Project Wizard, indicate that you want to “create new project at existing location” and then browse to set the Directory to the `sites` folder. Then name your project `famedev` at the top of the dialog. Hit the `Finish` button to complete the setup.
