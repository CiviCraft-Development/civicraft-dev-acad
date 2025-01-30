# Creating a Test Server

Test servers are core to the Minecraft plugin development process. They help developers troubleshoot their plugins, identifies bugs and other things that may have been overlooked, so that the plugin being put out has as little issues as possible. 

## Step 1: Download a Server Jar
There are many different server softwares to choose from, and you're welcome to choose which you prefer. Going forward, we'll be using Paper, but the following steps work with almost any other available server software.

### Go to <a href="https://papermc.io/downloads" target="_blank">PaperMC Downloads</a> 
Go to <a href="https://papermc.io/downloads" target="_blank">PaperMC Downloads</a> and download the latest build.

Throughout this tutorial, we'll be working on the latest version. However, if you'd like to develop on earlier versions, visit <a href="https://papermc.io/downloads/all" target="_blank">PaperMC's Build Library</a>, choose your preferred version, and download the latest build available for it.

### Rename the Downloaded File
After you've downloaded the server jar, rename it to `paper.jar`.

## Step 2: Create a Folder
Create a folder on your computer. You can decide where to create this folder, but we'll be creating it on our desktop for this lesson so that we have easy access to the folder. You can name this folder whatever you'd like!

### Place the Server Jar File into your Folder
With the folder created, place the 

## Step 3: Create a Batch File
This is the most error-prone step to the process. Make sure to follow along to the T!

### Create a Text File
Right-click in the server's directory and choose "New" then "Text Document". You can name this whatever you would like for now. Open up the text document and paste the following:
```
java -Xms128M -Xmx4000M -jar paper.jar nogui
PAUSE
```

Save the text document and go to your server folder. Rename the file to `run.bat`.

> The file extension is `.bat` so if your file is still `.txt` it will not work!


## Upgrading and Downgrading the Server
Upgrading and downgrading your test server is extremely easy once you have one already setup! Visit <a href="https://papermc.io/downloads" target="_blank">PaperMC Downloads</a> and download your preferred build. Once downloaded, navigate to the folder holding your server and delete the current `paper.jar`. Rename the newly downloaded build to `paper.jar` and place it in the server folder. The next time you start, and you’ll be running the new version!
