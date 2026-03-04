![dont-starve-together-steam-deck-bazzite-gamemode-notigv](https://github.com/user-attachments/assets/7071955b-3179-4dd1-8eb4-d9b4e64dd5ee)

# Don't Starve Together Resolution on Bazzite / Steam Deck (Docked) Fixed
**By NotiGV**

A simple fix for the Handheld Mode / 720p lock when playing docked on Bazzite or Steam Deck. Includes settings for 1080p, 1440p and Ultrawide monitors. :D

---

## 🛑 The Problem
If you play Don't Starve Together on Bazzite or a docked Steam Deck, you might have noticed the game gets stuck in Handheld Mode.

This locks the internal resolution to 720p (1280x800), making the game look blurry or creating giant black bars on your monitor, regardless of what you change in the Steam Properties.

This guide provides the definitive fix using **gamescope** to force the correct resolution! :D

---

## 🛠️ The Solution (Launch Options)
We need to bypass the game's hardware detection by forcing a specific window size before the game even starts.

1. Go to your **Steam Library**.
2. Right-click **Don't Starve Together** -> **Properties**.
3. In the **General** tab, find **Launch Options**.
4. Copy and paste the command below that matches your monitor:

**For 1080p Monitors:**
```bash
gamescope -w 1920 -h 1080 -W 1920 -H 1080 -f -- %command%
```

**For 1440p (2K) Monitors:**
```bash
gamescope -w 2560 -h 1440 -W 2560 -H 1440 -f -- %command%
```

---

## 🖥️ For Ultrawide Users (21:9)
If you are using an Ultrawide monitor (like 3440 x 1440), use this command instead. It will fix the aspect ratio and let you see much more of the map! :D

**For Ultrawide (3440 x 1440):**
```bash
gamescope -w 3440 -h 1440 -W 3440 -H 1440 -f -- %command%
```

**Note for Ultrawide:** The Main Menu might still have black bars on the sides because it's a static image. Don't worry! Once you load into the actual world/gameplay, the camera will zoom out and fill the entire screen perfectly.

---

## 🎮 Extra Tips
**Fixing the HUD on High Resolutions:** If your Health and Hunger meters feel too far away in the corners of your screen, I highly recommend installing the **"Combined Status"** mod from the Steam Workshop. It centers your stats and makes them much easier to read on big screens.

Hope this helps!! :D

---

## 📖 Read the Full Guide
If you prefer to read this guide with rich formatting, see the step-by-step screenshots, or want to drop a comment to the community, check out the official Steam version right here:

**[Read and Favorite the Official Steam Guide Here](https://steamcommunity.com/sharedfiles/filedetails/?id=3641850491)**

---

> ***Disclaimer:*** This technical guide was written and formatted by NotiGV to help the Linux and handheld gaming community optimize their displays. Technical Note: The gamescope launch options provided are standard system-level commands used to override resolution scaling on SteamOS/Bazzite. While they are completely safe, applying custom launch options is always done at your own discretion. Don't Starve Together is property of Klei Entertainment.
> 
> ***Editing Process:*** Digital creation and language assistance tools were utilized during the final proofreading of this guide to ensure clear, concise, and accurate technical instructions.
