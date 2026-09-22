# Team Frotress 2

Controls smart sex toys based on kills, deaths, and uber in Team Fortress 2, using the Intiface Central backbone to connect to hardware

Uber tracking requires the use of the OMPHUD-sexy edit

WARNING - Use only in private lobbies / servers with consenting players, and test your strengths before using them. The default values are ad-hoc and not suitable for every person or device

# Features
- Custom vibration strength and time for kills, death, using Uber, and passing milestones of Ubercharge percent
- Multipliers for critical kills, killstreaks, and "Uberstreaks"
- Execute custom TF2 console commands when vibration starts and stops

# Planned features
- Support for further features involving config file scripting, such as weapon & class specific functionality
- Support for assist tracking features (if anyone knows a good way to do this please reach out!)

# Setup

Copy config_default.py to config.py (you will have to create this file in the same directory as config_default.py) and fill out your game executable and console.log paths (console.log will be in tf
folder)

If you want medic functionality, install OMPHUD-sexy on your game, make sure every class config has `$classname` in it somewhere, i.e. medic.cfg has a
line `$medic`, heavyweapons.cfg has a line `$heavyweapons`. 

If you want hit detection functionality you will need to manually create an empty file called `hitsound.wav` file at `/tf/custom/test/sound/ui/hitsound.wav`, the console error this throws allows us to detect hits, this unfortunately disables the in-game hitsound so is optional.

Note that usernames with non-ascii characters cannot be used at the moment.

# Customising for multiple devices/motors

Edit the run_buzz method in vibration_handler.py to your liking


