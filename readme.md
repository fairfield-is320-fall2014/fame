#Developer Docs#

##Cloning from GitHub##
The following assumes you are using AMPPS and Eclipse, though the steps are likely similar for other development environments. 

1. Download and extract a copy of Drupal to your AMPPS `www` folder. 
2. Rename the folder you just extracted to `famedev`. 
3. Delete the `sites` folder from `famedev`. 
4. Open Eclipse. You should be in the PHP Perspective.
5. Select `File-->Import...` and then from the dialog choose `Git-->Project from Git ...`. Hit the `Next` button to continue.
6. Choose `Clone from URI` and hit `Next` to continue. 
7. Enter the URI `https://github.com/fairfield-is320-fall2014/fame.git` and select the `https` protocol. If you want to push changes back to GitHub then you will need to also set your GitHub username and password. 
Hit the `Next` button to continue. 
8. Select the `master` branch and hit `Next`.
9. Use the browse button to set the Directory to the `famedev` folder.
10. Eclipse will automatically add `fame` to the end of the Directory. Change `fame` to `sites` instead. Hit the `Next` button to continue. Watch as it downloads all the files to the new sits folder. 
11. Select the New Project wizard. Hit the `Finish` button to continue.
12. Within the New Project Wizard, indicate that you want to a `Create new project at existing location` and then browse to set the Directory to the `sites` folder. Then name your project `famedev` at the top of the dialog. Hit the `Finish` button to complete the setup.


##Configuring your local copy##
Once you have completed the steps above, you will then need to set up a database in phpMyAdmin.

1. Navigate your browser to `http://localhost/ampps/index.php?` and start phpMyAdmin within AMPPS.
2. Select `New` in the sidebar to the left and create a new database and name it "famedev".
3. Select your new database in the sidebar and select `SQL` from the navigation bar at the top of your screen.
4. Enter the following commands (note the punctuation and remember the semicolons) and then click `Go`:
* grant all on famedev.* to 'drupal'@'localhost' identified by 'drupal';
* flush privileges;
5. Go to `http://is-dsb.fairfield.edu/famedev/` and log in.
6. Select `Backup and Migrate` in the navigation bar at the top of your screen.
7. Click the link that reads `advanced backup page` and in there select `Download` from the `Backup Destination` dropdown menu. Click `Backup Now` and choose a place on your computer to download the .mysql file. This file will not need to be unzipped.
8. Go back into phpMyAdmin and back into your new, blank famedev database. Select `Import` from the navigation bar.
9. Click `Choose file` and select the .zip file you have just downloaded. Leave all other options on this screen as is and then click `Go`.
10. Navigate your browser to `localhost/famedev` to access your now-working local version of the site.
11. 

##Pulling changes from GitHub##
This section details how to pull from this GitHub repo from within Eclipse.

1. Start Eclipse and make sure you have the Project Explorer sidebar visible.
2. Right-click your "famedev" project and hover down to `Team` and then select `Pull`.
