# Awesome Thunderbird

After 10 years of frustration with Apple Mail. I am switching back to Thunderbird. Here are some customizations

## Contents
1. [News](#news)
2. [UI Changes](#ui-changes)
3. [Mouseless navigation](#mouseless-navigation)

## News
Started to work on a new version to support Thunderbird 115 (main branch now) 🐦

The latest working version for Thunderbird 102 can be found by checking out the branch b102 🕺🏽

## UI changes

Add this file to your Thunderbird chrome folder. For mac users this folder will be located at:

`~/Library/Thunderbird/Profiles/<<profile-folder>>/chrome`

What is contained in this file:

### Fonts

* Configurable font size for the interface
* Using SF Pro by default (Mac) instead of Verdana

### Reading mail
* mail list with alternating colors (I am old fashioned like that, when TB was awesome)


### General appearance changes
* message header buttons without borders (more streamlined imo)  
* warning messages appear in a toned-down blue (instead of the very bright yellow ugh!)

### Configurable styles
I am using CSS variables extensively with the goal of easing updating / creating different styles.

## Mouseless navigation

I a using the `tbkeys` plugin to interact with Thunderbird without the mouse, saving a lot of time as my hands never leave the keyboard, improving my email efficiency. Also trying to align my shortcuts here with Neovim (e.g. j -> down, k-> up...)

```json
{
    "j": "cmd:cmd_nextMsg",       
    "k": "cmd:cmd_previousMsg",   
    
    "o": "cmd:cmd_openMessage",
    "c": "func:MsgNewMessage",
    
    "d": "cmd:cmd_delete",
    "a": "cmd:cmd_archive",
    "s": "cmd:cmd_markAsJunk",
    
    
    "v": "MsgMoveMessage('imap://<!-- your spam folder goes here  -->/Spam')"
    "u": "tbkeys:closeMessageAndRefresh",
}
```





