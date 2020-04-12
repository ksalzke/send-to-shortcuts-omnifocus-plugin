# About

This is an Omni Automation solitary plug-in for OmniFocus that sends details of a selected task to Shortcuts (in JSON format). (This plug-in was created largly for demo purposes.)

**Note that if you are working with Shortcuts and OmniFocus, you may also consider OmniFocus' new Shortcuts actions as an alternative option: depending on your needs, they may be easier to work with than this script.**

_Please note that Omni Automation for OmniFocus is still in development and details are subject to change before it officially ships. If you have questions, please refer to [Omni's Slack #automation channel](https://www.omnigroup.com/slack/)._

_In addition, please note that all scripts on my GitHub account (or shared elsewhere) are works in progress. If you encounter any issues or have any suggestions please let me know--and do please make sure you backup your database before running scripts from a random amateur on the internet!_

## Known issues

None so far! 🤞

# Installation & Set-Up

(For instructions on getting started with Omni Automation, see [here](https://kaitlinsalzke.com/how-to/how-to-add-a-omnijs-plug-in-to-omnifocus-and-assign-a-keyboard-shortcut/).)

1. Click on the green `Clone or download` button above to download a `.zip` file of the file in this GitHub repository.
2. Unzip the downloaded file.
3. Move the `.omnijs` file to your OmniFocus plug-in library folder.
4. Update the `shortcutToRun` variable to the name of the Shortcut that is to receive the information.

# Actions

## Send To Shortcuts

This action sends information about a selected task (in JSON format) to the Shortcut specified in the `shortcutToRun` variable (by default "Receive Data From OmniFocus").

The first step in the Shortcut needs to be `Get Dictionary From Input` and then you can use the information like any other dictionary. (You can see an example [here](https://www.icloud.com/shortcuts/d6e300fba0714f748e2a90c1eaabefd3), which simply gets the dictionary and then displays it.)

Currently it sends the following information:
* name
* project name
* tags
* defer date
* due date
* flagged
* note
* ID