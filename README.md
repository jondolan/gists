# My Gists
A list of my [Github gists](https://gist.github.com/jondolan/) to provide more details about those scripts.


## [AutoHotkey Windows drop down terminal script](https://gist.github.com/jondolan/9eb0a9eefffac3ae67445763973e9f58)
Using [AutoHotkey](https://autohotkey.com), I mimicked drop down terminal functionality provided by the popular Unix packages [Guake](http://guake.org/)/[Yakuake](https://en.wikipedia.org/wiki/Yakuake). As someone who regularly switches between Linux Mint and Windows, using F12 to summon my terminal is second nature and severely missed while in Windows.

To use this script yourself, I would recommand installing AutoHotkey, downloading my Gist, and right clicking on the file selecting "compile script." You can also just download the compiler separately, or not compile the script and just use AutoHotkey directly.

I place the compiled script in my Windows user startup folder (C:\Users\<user name>\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup). The script does nothing if a terminal session with matching window title is not already opened.


To configure it for your usage, you must modify the variables from line 23 "GLOBAL VARIABLES" and down.

- **win_title** allows you to specfiy a unique substring in the title of the window of the program you are aiming for.
- **win_width_percent** and **win_height_percent** allow you to specfiy how much of your computer's screen the drop down terminal should occupy.
- **win_visible_transparency** allows you to specify from 0 (completely transparent) to 255 (opaque) the transparency of the drop down window when it is visible. I use this so I can read text underneath the terminal when it's open

&nbsp;

## [Outlook browser notifications](https://gist.github.com/jondolan/634cbcb40b252659a4b71c1b89b800ef)
This is a Javascript based [UserScript](https://userscripts-mirror.org/) which converts the Outlook.com in-window email notification to a native browser notification (supported by Chrome and Firefox).

This is useful because the standard Outlook.com email notifications are only visible if you have the page open, which has absolutely 0 utility. The script monitors for the presence of these notifications, and then converts it into a native notification.

You must "allow browser notifications" from Outlook.com when prompted after first loading the script.

I personally use the [Tampermonkey](https://chrome.google.com/webstore/detail/tampermonkey/dhdgffkkebhmkfjojejmpbldmpobfkfo) Chrome extension to load my UserScripts.

&nbsp;

## [Google Calendar small window style fixer](https://gist.github.com/jondolan/2f656790de0e4fdbd086645efe22032c)
Not much to see here, just a lazy userscript that modifies the style of some elements of the Google Calendar webpage to suit my needs better when I put it on a 3 day view and let it occupy ~1/5 of my screen with email on the other side.
