![dont-starve-together-steam-deck-bazzite-gamemode-notigv](https://github.com/user-attachments/assets/7071955b-3179-4dd1-8eb4-d9b4e64dd5ee)

# Don't Starve Together Resolution on Bazzite / Steam Deck (Docked) Fixed
**By ThatGVguy**

A simple fix for the Handheld Mode / 720p lock when playing docked on Bazzite or Steam Deck. Includes settings for 1080p, 1440p, and Ultrawide monitors. And believe me, it's a very simple fix! ;)

---

## 🛑 The Problem
If you play **Don't Starve Together** on Bazzite or a docked Steam Deck, you might have noticed the game constantly gets stuck in Handheld Mode.

This annoying bug locks the internal resolution straight to 720p (1280x800), making the game look incredibly blurry or creating giant, ugly black bars on your external monitor—completely ignoring whatever you try to change in the standard Steam Properties menu!

This guide provides the definitive fix using **gamescope** commands to force the correct resolution and save your eyes! :D

---

## 🛠️ The Solution (Launch Options)
We need to bypass the game's hardware detection by forcing a specific window size before the game even starts. Here is exactly what you need to do:

1. Go to your standard Steam Library layout.
2. Right-click **Don't Starve Together** and select **Properties...** from the context menu.
3. In the **General** tab, look for the **Maximum Game Resolution** option and change the dropdown menu to **Native**.

![Dont Starve Together-steam-deck-bazzite-gamemode-thatGVguy 2](https://github.com/user-attachments/assets/e8bcba29-7216-46fd-8826-32cd07cbd0ad)

> ⚠️ **Crucial Step Note:** This is super important! It completely ensures the game boots up using your external monitor's exact resolution instead of scaling up a smaller, stretched image! Don't skip it! :D

4. Scroll down just a tiny bit on that same tab to find the **Launch Options** input field box at the bottom.

![Dont Starve Together-steam-deck-bazzite-gamemode-thatGVguy](https://github.com/user-attachments/assets/2ffdca16-11c5-418e-8251-19c5f73e2e79)

5. Copy and paste the exact command line string below into the box:

```bash
Steamdeck=0 %command%
```

---

## The Last Step: In-Game Settings (Super Important!)

We are almost there! Once you have placed the command string and changed the resolution option in Steam, we just need to do one last quick thing inside the game itself to make everything work perfectly. Just follow these simple steps:

**1. Launch the game:** Launch the game normally and go straight into **Options** from the main menu


<img width="2560" height="1440" alt="Dont Starve Together-steam-deck-bazzite-in game-thatGVguy" src="https://github.com/user-attachments/assets/a7c1a058-0a6e-4fe6-b57f-e7f287505f35" />

**2. Access graphics menu:** On the left sidebar menu, head over to the **Graphics** tab.


**3. Adjust resolution and FPS:** Now, change the **Resolution** and **Refresh Rate** to match the exact native resolusion of your external monitor. Make sure to pump those Hz up to your monitor's max limits so the gameplay feels ultra smooth!! :D


<img width="2560" height="1440" alt="Dont Starve Together-steam-deck-bazzite-in game options-thatGVguy" src="https://github.com/user-attachments/assets/6deeebdb-5e8d-417b-ba9f-a859c976c7e1" />


**4. Apply and accept:** Click the **Apply** button at the bottom. A tiny confirmation box will pop up, click **Accept** and you are completely done! The game will shift to that crisp resolution instantly

<img width="2560" height="1440" alt="Dont Starve Together-steam-deck-bazzite-in game options 2-thatGVguy" src="https://github.com/user-attachments/assets/b25061d7-55ef-41b2-a243-001b1fca1a3e" />

---

## 🖥️ For Ultrawide Users (21:9)
If you are using an Ultrawide monitor (like a 21:9 setup or 3440 x 1440), use the exact same command string! It will instantly fix the aspect ratio and let you see much more of the constant dangers on the map! :D

> **Note for Ultrawide Users:** The Main Menu might still display black bars on the sides because it is a fixed, static image asset. Don't panic, this is completly normal!

![Dont Starve Together-steam-deck-bazzite-gamemode-thatGVguy-ultrawide](https://github.com/user-attachments/assets/6a905ef0-9aa2-4ba9-9e3d-fa51320a2b43)

Don't worry at all! The very second you load into the actual world and start the active gameplay, the camera will zoom out seamlesly and fill your entire display perfectly. Enjoy the massive view!

![Dont Starve Together-steam-deck-bazzite-gamemode-thatGVguy-ultrawide2](https://github.com/user-attachments/assets/741e3ec7-21e4-471f-a4a4-be00762abbf3)

---

## 🎮 Extra Tips: Fixing the HUD on High Resolutions
If your Health, Sanity, and Hunger meters feel way too far away in the distant corners of your screen, I highly recommend installing the legendary **"Combined Status"** mod directly from the Steam Workshop. 

It beautifully centers your stats, displays exact numbers, and makes them infinitely easier to read on big screens without straining your eyes. This is highly usefull specialy if you are sitting a bit far away from your docked setup!

🔗 **Get the Mod Here:** [Combined Status (Steam Workshop)](https://steamcommunity.com/sharedfiles/filedetails/?id=376333686)

Hope this helps you survive out there!! Don't starve, and enjoy your crisp native resolution layout! :D

### FPS Stuck at 60?
Cant change the refresh rate when saving? If you want to play at more than 60 FPS but the game keeps reseting your choice back to 60, you will need to do one quick extra step!!

1. Switch over to **Desktop Mode**

2. Open your terminal (Konsole) and type the following command to find your config file:

<img width="984" height="568" alt="Dont Starve Together-steam-deck-bazzite-fps-thatGVguy" src="https://github.com/user-attachments/assets/7e2b86ec-eb2d-416c-a30c-145d34bdb4fe" />
 
   `find ~ -type f -name "client.ini" -path "*/DoNotStarveTogether/*"`

3. This will spit out a file path. It will look something exactly like this:

   `/home/[YOUR_USER]/.local/share/Steam/steamapps/compatdata/322330/pfx/drive_c/users/steamuser/Documents/Klei/DoNotStarveTogether/[YOUR_STEAM_ID]/client.ini`

4. Copy that exact path and paste it directly into Dolphin's (your file manager) address bar. This will open the configuration text file.

<img width="2560" height="96" alt="Dont Starve Together-steam-deck-bazzite-dolphin search-thatGVguy" src="https://github.com/user-attachments/assets/ea986197-4a7f-4c5e-9b9e-f4f30370e753" />

5. Search for the `refresh_rate` line in there and change the `60` to the maximum FPS number of your monitor.

<img width="1394" height="1167" alt="Dont Starve Together-steam-deck-bazzite-fps ini-thatGVguy" src="https://github.com/user-attachments/assets/75375a9f-1ab7-49fb-a6d5-d2a85e799b6a" />

6. Hit **Save** on the file and close it.

And with that, you will finaly have the crisp resolution and the ultra smooth FPS you always wanted! :D

---

## 📖 Read the Full Guide
If you prefer to read this guide with rich formatting, see the step-by-step screenshots, or want to drop a comment to the community, check out the official Steam version right here:

👉 **[Read and Favorite the Official Steam Guide Here](https://steamcommunity.com/sharedfiles/filedetails/?id=3641850491)**

---

## 📜 Codex Umbra: Technical Notes & Credits

* **The Goal:** This technical guide was written and formatted by me, **ThatGVguy**, to help our awesome Linux and handheld gaming community optimize thier external displays. No more blurry graphics or giant black bars on your beautiful monitors!
* **Technical Note:** The gamescope launch options provided here are standard system-level environment variables used to override hardware detection on SteamOS/Bazzite. While they are completely safe to use, applying custom launch choices is always done at your own discretion. *Don't Starve Together* and all its creepy monsters are the exclusive property of the legends at **Klei Entertainment**.
* **The Final Proofread:** To guarantee a clear, concise, and highly accurate reading experience for everyone, digital creation and language assistence tools were utilized during the final proofreading phases of this text. The trick works perfectly, and the formatting help just makes it look nice and scannable!

> Now go out there, build your base, and enjoy the beautiful full view of the Constant! 🌲🎒
> — **ThatGVguy :D**
