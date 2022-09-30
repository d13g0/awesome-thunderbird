# Awesome Thunderbird

After 10 years of frustration with Apple Mail. I am switching back to Thunderbird. Here are some customizations

## Contents

1. [UI Changes](#ui-changes)
2. [Mouseless navigation](#mouseless-navigation)


## UI changes

Add this file to your Thunderbird chrome folder. For mac users this folder will be located at:

`~/Library/Thunderbird/Profiles/<<profile-folder>>/chrome`

What is contained in this file:

* Configurable font size for the interface
* Using SF Pro by default (Mac) instead of Verdana
* mail list with alternating colors (I am old fashioned like that, when TB was awesome)
* message header buttons without borders (more streamlined imo)  
* warning messages appear in a toned-down blue (instead of the very bright yellow ugh!)

Also:

I am working on using CSS variables with the goal of easing updating / creating different styles.

Next in my list:

* Dark mode 


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

