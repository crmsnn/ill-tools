# Ill tools
A compilation of tools for making impossible levels in Geometry Dash, focused on version 2.1 of the game.

https://www.impossiblelevels.com

https://discord.gg/MHx4Nbp

Main sources are ILL pins, ICL #gd-resources and crmsn's #tools.


I'm currently looking into hosting some of the .dlls in this repo, I just need to check permissions.

***
# Getting Older versions

### Depot Downloader

Im my opinion, depot downloader is the best way to get older version

**Windows setup:** Press Win+R to open Runner, paste in this command:
```
steam://open/console
```

**Linux setup:** Close steam if it's open, and run the command:
```
steam -console
```

**2.1 download command:**
```
download_depot 322170 322171 641118531549408775
```
Robtop seems to have disabled signing into older versions, you can still build though.
If you're already logged into 2.1 somewhere, you can copy CCGameManager.dat

**Depot commands for other versions:**
```
download_depot 322170 322171 7903404280228366327 for 2.206

download_depot 322170 322171 2530486154587189554 for 2.204

download_depot 322170 322171 8259882692733807559 for 2.203

download_depot 322170 322171 2018952014081804638 for 2.202

download_depot 322170 322171 6284244757349794393 for 2.201

download_depot 322170 322171 3500860979376500740 for 2.200

download_depot 322170 322171 641118531549408775 for 2.11

download_depot 322170 322171 4058039153940377450 for 2.10

download_depot 322170 322171 631879647548207429 for 2.02

download_depot 322170 322171 542142667514100820 for 2.01

download_depot 322170 322171 2135166447199899913 for 2.00

download_depot 322170 322171 1039208287639585563 for 1.921

download_depot 322170 322171 4586891070648157831 for 1.91 
```

**RENAME THE .EXE IT CONTROLS WHERE SAVE DATA IS STORED AND CAN WIPE YOUR DATA**


Otherwise, there's
### GDPSs
Not as seemless as depot downloader in my experiences, but it does work.

**GDPS Hub:**
https://gdpshub.com/

You can also surf Youtube & Discord, but I won't be providing links to either.

**Be aware that some GDPS check if you have steam & GD already**

Always make sure there is a `steam_appid.txt` file with the text `322170` inside the folder
***
# General Mod menus

**(Universal) Cheat Engine:**
https://www.cheatengine.org/

### 2.2

Geode is without a doubt the best choice, being a full on mod ecosystem.

https://geode-sdk.org/

Within Geode, the common consensus is that **Eclipse** and **Silicate** are the best currently available

**yBot:**
https://ybot.store/

**TCbot/ծBot:**
https://www.tcbot.pro/

**Silicate:**
https://discord.gg/dFfNGW2V

### 2.1

**Mega Hack v7:**
https://absolllute.com/

**MHV7 on linux:**
https://www.youtube.com/watch?v=EYQBQ4xNb_0

**GDHM:**
https://web.archive.org/web/20230402215601/https://adaf.xyz/adaf/hm/download/v35.6/8705cae3fff101c2bb6c884f5c68bda983c0955d7fa477692424cd2c727cafea/GDHM_TASBOT_v35.6.zip

Instalation Guide:
https://docs.google.com/document/d/1OHlalyltq6is6o8EfYCVqeZBiBVWcEea/edit?usp=sharing&ouid=100518803770411660850&rtpof=true&sd=true


**GDMO:**
https://github.com/maxnut/GDMegaOverlay/releases/tag/1.41

**GDH:**
https://github.com/TobyAdd/GDH/releases/tag/v1.3.1

### 2.0

**PolzHox 2.0:**
https://github.com/Pololak/PolzHax-2.0

### 1.9

**PolzHox**
https://github.com/Pololak/PolzHax

### Mobile

**iCreate Pro:**
https://icreate.pro/

# 2.1 Mods & Extensions

*This is by no means a comprehensive list*

**Echo 1.1:**
https://cdn.discordapp.com/attachments/838145374849204244/1178573916088836106/Echo_v1.1.dll?ex=688c55fe&is=688b047e&hm=ff19c915bd331885fc40001fe3dbc820dee72fad41bb1514ca410ce0e71f93bc&

**Obot v3:**
[Link](https://cdn.discordapp.com/attachments/1400491385928417330/1419721329774559293/OmegaBot_3.1.2_x64-setup.exe?ex=69043a46&is=6902e8c6&hm=eb76eb2511c9b0f068b266db81f4e55e60c54f21170859b3dc378e1c626fa5b7&)

**GD Share:**
https://github.com/HJfod/GDShare/releases/tag/v0.3.4

**Better Edit:**
https://github.com/HJfod/BetterEdit/releases/tag/v4.0.5

**Sai Mod Pack:**
https://www.mediafire.com/file/07jh86czbpf9dtm/Sai_Mod_Pack_-_v1.5.zip/file

**Better Pause:**
https://github.com/TpdeaX/BetterPause/releases/tag/Release

**Separate Dual Icons:**
https://github.com/Alphatism/SeparateDualIcons/releases/latest

**Mat's Mods:**
https://matcool.github.io/mods

# Useful videos

**Frame Alignment Explained by HaydenDom:**
https://youtu.be/WjCs2HQ3CRA

**How To Make A Frame Gate by Locked101:**
https://www.youtube.com/watch?v=dBaRtDLln8Q

# Miscellaneous

### Showcaseing tools

**Rendering software some bots need:**
https://github.com/absolllute/ffmpeg-build/releases/tag/v1

**doki and nvi's 4k guide**

codec: `h264_nvenc` (nvidia) / `h264_qsv` (intel quicksync) / `h264_amf` (amd) / `libx264`
-# use `hevc_nvenc` if you have a newer nvidia card
resolution: 3,840 x 2,160
bitrate: `200` (mbps)

args main:
`-pix_fmt yuv420p -preset fast -crf 8`
// raise crf to -crf 10 if you do not require ridiculously high quality (recommended for editing and processing the video in a video editor) - look at nvi's message for further detail

args vf:
`colorspace=all=bt709:iall=bt470bg:fast=1`
// colour fix, very important

args audio:
`-c:a libmp3lame -b:a 320k`
// raises audio quality to 320kbps (very recommended)

**wndy's Doc:**
https://docs.google.com/document/d/196ft5_d-BB88G9FftS4hPPrMEJGIfWdp-j3Y5_hJxfs/edit?usp=sharing


### Glowfix

*Uneeded past 2.1*

Download a hex editor:
**HxD (Windows):**
https://mh-nexus.de/downloads/HxDSetup.zip

*If you're on linux get Bless*

Drag GeometryDash.exe into the window

Press ctrl+g and then type "3c1f7"
*in bless you need to search for 0x3c1f7*

Change the 06 to 00

Download and replace https://www.dropbox.com/s/apv7n1dqb5hxo0w/GJ_GameSheet-uhd.png?dl=0 in resources

### 4gb patch

https://ntcore.com/4gb-patch/

### Macro tools

**Macro type converter:**
https://conv.nattie.dev/

**Cps checker:**
https://mumbles246.github.io/cpsChecker/

### GMD tools

Backporting 2.2 to 2.1
https://gdcolon.com/gmd_tools
