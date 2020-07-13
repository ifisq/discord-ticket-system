# Auroris Ticketing Bot

This is a Discord bot meant to handle tickets for a server. 

## Steps to Install:

1. Download python from https://www.python.org/downloads/
2. Run the installer.
3. Go into command prompt and enter the following code command

      **Windows:** `py -m pip install discord asyncio`

      **MacOS:** `python3 -m pip install discord asyncio`

4. Go to https://discordapp.com/developers/applications and create your application, go to the bot section, and copy your token. Place it into the quotes on the last line of code in main.py, replacing the word **TOKEN**. 
5. Go back to command prompt, and cd (navigate) to the directory where you've downloaded this project. Run the following command once you are in the directory on command prompt:

      **Windows:** `py main.py`
      
      **MacOS:** `python3 main.py`
  
6. Success! If you see the bot saying that it's running with your username and user ID displayed, you've successfully setup the bot.

## How to configure the bot

There's a variety of commands for administrators to use to configure the bot. The features that you can customize are what roles have access to ticket channels, what roles get pinged when a new ticket is created, and what users can configure the previous options. An important distinction to make is between users who have admin-level permissions for the bot and users who have administrative level permissions for the entire server. In order to provide more customizability, I've incorporated a special subset of roles that can be configured in order to have access to the commands to add/remove roles from tickets and to add/remove roles that get pinged in tickets. That may sound a bit confusing, but here's how it works:

A user with administrator level permissions sets the bot up. He automatically has access to every single command that the bot offers. However, he may have a few trusted moderators with a Moderator role that he wants to have access to add roles that can be pinged, or to add specific roles to tickets. He can do this via the `.addadminrole` command. This command gives these users access to all of the commands that the actual administrator has, but they do not gain administrative permissions for the *entire* server. 

## Questions/Bugs/Suggestions?

If you have any suggestions for additions to the bot, find any bugs, or have any questions, feel free to open an issue or message me on Discord and I'll take a look at it. For updates, follow me on [Twitter](https://twitter.com/ifisq).
