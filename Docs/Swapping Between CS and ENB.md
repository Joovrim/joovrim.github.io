---
title: Swapping Between CS and ENB
layout: home
nav_order: 7
---

# So you want to try out ENB and see if you like it better?


Well I will admit that for my own sanity I made it a little harder but in exchange I will walk you through swapping between the two step by step as clearly as I can

## Step 0 - Good Modding Practices


The first thing you are going to do is prepare for if you either want to go back or if you mess something up. To do this we are going to clone the current profile. Simply open your Tahrovin MO2 instance, click the person/ID icon at the top left, click your current profile and then click copy. Name the new profile whatever you want. Select the new profile from the dropdown at the top of the left side of MO2 and work on that profile, if you mess things up, delete the profile, clone the original again, and start over on the clone.


## Step 1 - Enabling Mods


(In this guide I will be swapping from CS to ENB but you can also do the reverse.)
1. Go to the For Tahrovin ENB Subheader
2. Enable the following mods:
    - Tahrovin enbseries binaries
    - ENB Helper VR
    - VR Parallax Shader Fix
    - ENB Helper Plus
    - Skyrim VR OpenComposite ENB fix
3. Choose which ENB you wish to try, for this example I will be using Rudy as it is the most complicated
4. activate your chosen ENB (for Rudy enable both Rudy ENB Cathedral Weathers ADDONS and REQUiRED Files and Rudy Zangdar ENB for Cathedral Weathers - VR Tweaks)

Your For Tahrovin section should now look like this except for your ENB choice.

![ENB Swap 1](/assets/images/ENB%20Swap%201.png)

5. Head down to the Weather Stuff subheader and enable Cathedral Weathers and Seasons (ENB) ***DO NOT DISABLE ANY MODS YET***
6. Head down to the Tahrovin Custom Patches & Stuff subheader and enable Tahrovin ENB weather patch


## Step 2 - Sorting the esp plugins


We will now use CS and its plugins as a guide for where to put ENB's plugins
1. In the Plugins Pane on the right side of MO2 Filter for weather
2. Note Real VR weather's priority and right click cathedral weathers and click send to, then priority, and send it to the priority you noted earlier

![ENB Swap 2](/assets/images/ENB%20Swap%202.png)

Mine is 277, yours may be different.

![ENB Swap 3](/assets/images/ENB%20Swap%203.png)

3. Place Tahrovin ENB patch.esp just below TahrovinCSPatch.esp
4. Place Cathedral Weathers Godrays.esp just below Tahrovin ENB Patch.esp
5. ***Rudy ENB Only*** Place NightEyeENBFix.esp just below Cathedral Weathers Godrays.esp
6. ***Rudy ENB Only*** place Cathedral Weathers - Patch - Rudy ENB.esp just under NightEyeENBFix.esp

It should now look something like this

![ENB Swap 4](/assets/images/ENB%20Swap%204.png)


## Step 3 - Disabling Mods


Now we begin the process of disabling CS, it's weather, and it's plugins
1. In the subheader Tahrovin Custom Patches & Stuff disable Tahrovin Community Shaders Patch
2. In the subheader Weather Stuff disable Real VR Weathers (Community Shaders)
3. In the subheader CS Resources disable everything ***EXCEPT FOR Auto parallax and Auto parallax true ini***


## Step 4 - Test


If you have successfully enabled ENB you should be able to test it by running Tahrovin and then hitting Shift+Enter while in desktop mode with the window in focus to open the menu.

***If you are trying to do this in reverse to swap from ENB to CS and you cant get the CS menu to reappear you may need to clear your overwrite folder by right clicking overwrite at the bottom of MO2 and clicking clear***

![ENB Swap 5](/assets/images/ENB%20Swap%205.png)

Congrats you should now be all swapped!

You did remember to backup your profile in case you want to go back right?


