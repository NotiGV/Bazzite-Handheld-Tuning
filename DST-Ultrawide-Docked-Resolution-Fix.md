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
