# Installing MongoDB

## macOS Instructions:
Install MongoDB using Homebrew using the following commands:

```
brew tap mongodb/brew
```

The above command might take a moment or two to complete. When finished, install MongoDB with:

```
brew install mongodb-community
```

### Starting the MongoDB Server
You start the Mongo database server with the following command:

```
brew services start mongodb-community
```

The above command also ensures that the MongoDB engine runs after restarting your computer.

More info about installing MongoDB using Homebrew can be found [here](https://github.com/mongodb/homebrew-brew).

## Windows Subsystem for Linux (WSL) Instructions 

Install MongoDB using apt using the following command:

```
sudo apt install mongodb
```

### Starting the MongoDB Server
You start the Mongo database server with the following command:

```
sudo service mongodb start
```

Note: You will need to re-run this command after you reboot your machine to restart the mongodb service!


## Windows Powershell Instructions:
Install the MongoDB .msi installer from the website [here](https://www.mongodb.com/try/download/community?tck=docs_server).


### Add the `bin` folder to PATH

1. Find your `bin` folder. Most likely ot will be in `C:\Program Files\MongoDB\5.0\bin`

    ![Program Files](https://i.imgur.com/iiBWVmW.png)

2. Copy the path to the bin folder then bring up the "System Properties" window. To bring it up, search for "Edit the System Environment Variables" in the Start menu.

    ![Edit the system environment variables](https://i.imgur.com/lz9VYaV.png)

    ![System Properties](https://i.imgur.com/7JrnGsH.png)

3. Click on "Environment Variables in the System Properties Menu.
4. Click on "PATH" under "User variables"
5. Click on the "Edit" button
    ![Environment Variables](https://i.imgur.com/wZfwwsT.png)

6. Click on the "New" button in the "Edit environment variable pop-up menu and paste in the path to the `bin` folder.
    ![PATH](https://i.imgur.com/FzgEpBL.png)

7. Restart Powershell, and try running the `mongo` command!