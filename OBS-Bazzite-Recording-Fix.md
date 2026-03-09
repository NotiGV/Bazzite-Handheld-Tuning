![obs-recorder-steam-deck-bazzite-gamemode-notigv](https://github.com/user-attachments/assets/dcab4258-e8d8-4afa-a934-c88ee3f6d5b7)

# Record and Stream with OBS on Bazzite / Steam Deck (Game Mode)
**By NotiGV**

A fast, no-nonsense guide to using OBS Studio inside Game Mode. Perfect for recording at max quality, fixing a broken Steam Game Recording or streaming straight from your console or PC with Bazzite! :D

**Includes:**
* Step-by-step OBS Studio and OBS VkCapture plugin installation via Flatpak.
* How to fix the 21:9 Ultrawide resolution scaling and black screens.
* The exact Launch Options needed for native Steam games and Emulators (Dolphin, PCSX2, DuckStation & More).

Let's get those epic clips!! :D

---

## 🛑 The Problem
This guide is made to fix the issue where the native Steam Game Recording is broken or glitchy. Also, you might want to stream your gameplay (which you can do with OBS and not with the Steam Recorder), or you just trust OBS and already have your scenes and settings ready! :D

The problem is that since Bazzite's Game Mode uses the **Gamescope** compositor, OBS cannot capture the full screen directly. If you try to record, you will just get a black screen. 

This guide provides the definitive solution to hook OBS directly into your games! :D

---

## 🛠️ The Solution (Installing OBS & Plugin)
Since Bazzite is an immutable system, we will install everything via Flatpak to keep it safe and clean.

### Step 1: Install OBS Studio
Go to Desktop Mode, open the Discover software center, search for OBS Studio, and install it.
*(Alternatively, open Konsole and type this command):*
```bash
flatpak install flathub com.obsproject.Studio
```

### Step 2: Install the OBS VkCapture Plugin
For OBS to see your games inside Game Mode, we need to install a bridge (plugin). Sometimes it doesn't show up in Discover, so the terminal is the fastest way! :D

Open your terminal (Konsole), paste this command and press Enter:
```bash
flatpak install flathub com.obsproject.Studio.Plugin.OBSVkCapture
```
*Note: If it asks whether to install as "User" or "System", always choose **System**.*

### Step 3: The Emulator Fix (EmuDeck / Flatpak Users)
If you use emulators like Dolphin, RetroArch, or DuckStation installed via EmuDeck or Discover, they live inside a Flatpak "sandbox" that blocks OBS from seeing the video. We need to give them permission by installing a specific capture layer.

Open your terminal (Konsole), paste this command and press Enter:
```bash
flatpak install flathub org.freedesktop.Platform.VulkanLayer.OBSVkCapture
```
If the terminal gives you a numbered list of versions (like 21.08, 24.08, 25.08...), type the number for the **highest/newest version** (for example, type `5`) and press Enter. Press `Y` to confirm the installation.

* **Tip for Emulators:** Make sure your emulator's Video Backend / API is set to **Vulkan** in its graphical settings, otherwise the capture plugin might not detect it!

Done! The magic is installed. :D

---

## ⚙️ Configuring OBS
Open OBS Studio. Now we need to add the correct source and tweak a few things to avoid cropping or a giant zoom on your screen.

1. In the Sources box, click the **+** button.
2. Select **Game Capture**. *(This option appears thanks to the plugin we just installed! :D)*
3. Right-click that source in the list -> **Transform** -> **Fit to screen**.

### 🖥️ For Ultrawide Users (21:9)
If you play on an Ultrawide monitor (like 3440x1440), OBS might crop your image if the canvas and output aren't set properly. Let's fix that! :D

1. Go to **Settings** -> **Video**. Change both Base (Canvas) Resolution and Output (Scaled) Resolution to `3440x1440`.
2. Go to **Settings** -> **Output** -> **Recording**.
3. **¡IMPORTANT!** Make sure the **Rescale Output** option is Disabled. If it's checked, it will ruin your 21:9 aspect ratio! :(
4. Use the **Hybrid MP4** format so your videos won't corrupt if the power goes out.
5. In Video Encoder, select **FFmpeg VAAPI AV1** (if you have an AMD card that supports it) for better quality at half the file size.

---

## 🚀 Launch Options
To make the game send its image to OBS, we have to tell Steam to do so. Go to your Steam Library, right-click the game -> **Properties** -> **General** -> **Launch Options**.

Depending on what you are trying to play, follow the rule that applies to you:

**Case 1: The box is completely empty**
This applies to almost all native Steam games (like Hollow Knight) and clean emulators (like PPSSPP or Ryujinx). Just paste this:
```bash
OBS_VKCAPTURE=1 %command%
```

**Case 2: The box already has %command% in it**
If you already have environment variables (like `vblank_mode=0 %command%` for Dolphin), don't delete them! Just put our command at the very beginning and leave a space:
```bash
OBS_VKCAPTURE=1 vblank_mode=0 %command%
```

**Case 3: The box has text, but NO %command%**
Very common in PCSX2 setups (e.g., `-fullscreen -batch`). Put our command AND the `%command%` variable at the very beginning, leaving a space before the original text:
```bash
OBS_VKCAPTURE=1 %command% -fullscreen -batch
```

---

## 🎥 Extra Tips: How to record in Game Mode
1. In Desktop Mode, open Steam -> click **Add a Game** -> **Add a Non-Steam Game** and select OBS Studio.
2. Go back to Game Mode, open OBS from your library, and click **Start Recording**.
3. Press the Steam button to leave OBS running in the background.
4. Launch your game and enjoy! Your GPU will do all the heavy lifting.

---

## 📝 Author's Note :D
Setting this up can seem daunting at first, but it is entirely worth it! Sharing high-quality gameplay is one of the best parts of the gaming community. Getting the configuration right just once lets you forget about the technical stuff and focus entirely on the fun later.

I'd love to hear what games you are excited to record or stream first on Bazzite in the comments below! Have fun recording your best moments! :D

---

## 📖 Read the Full Guide
If you prefer to read this guide with rich formatting, see the step-by-step screenshots, or want to drop a comment to the community, check out the official Steam version right here:

**[Read and Favorite the Official Steam Guide Here](https://steamcommunity.com/sharedfiles/filedetails/?id=3678225635)**

---

>***Disclaimer:*** This technical guide was written and formatted by NotiGV to help the Linux and handheld gaming community optimize their recording setups. 
>
> ***Technical Note:*** The environment variables and Flatpak commands provided are standard, safe system-level commands for Bazzite/SteamOS. Applying custom launch options is always done at your own discretion.
>
> ***Editing Process:*** Digital creation and language assistance tools were utilized during the final proofreading of this guide to ensure clear, concise, and accurate technical instructions.

*Happy recording, and I'll see you on stream! :D*
