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

![bazzite-steamos-steamdeck-OBS-interface-gamode-notigv](https://github.com/user-attachments/assets/93b031d9-2643-4d0d-9d3b-26346f2080d1)

This guide provides the definitive solution to hook OBS directly into your games! :D

![bazzite-steamos-steamdeck-OBS-interface-gamode-games-notigv](https://github.com/user-attachments/assets/1cdd5836-3a24-49b4-80bf-a38f8863e836)

![bazzite-steamos-steamdeck-OBS-interface-gamode-games-AA-notigv](https://github.com/user-attachments/assets/fd147511-e2a2-4caf-b041-6d7a2bc7e68c)

---

## 🛠️ The Solution (Installing OBS & Plugin)
Since Bazzite is an immutable system, we will install everything via Flatpak to keep it safe and clean.

### Step 1: Install OBS Studio
Go to Desktop Mode

![bazzite-steamos-steamdeck-OBS-interface-kde-notigv](https://github.com/user-attachments/assets/62edeed1-deec-4b24-836d-0ef2d1e87f7d)

Open the Discover software center

![bazzite-steamos-steamdeck-OBS-interface-discover-notigv](https://github.com/user-attachments/assets/0e80fed3-c083-4633-b3a1-521081ddd451)

![bazzite-steamos-steamdeck-OBS-interface-discover-interface-notigv](https://github.com/user-attachments/assets/b1500b2f-0a8d-48c3-b36e-249b28404a06)

![bazzite-steamos-steamdeck-OBS-interface-discover-interface-options-notigv](https://github.com/user-attachments/assets/51853db8-5cc4-49de-9731-64d01afdca66)

Search for OBS Studio, and install it.

![bazzite-steamos-steamdeck-OBS-interface-discover-OBS-notigv](https://github.com/user-attachments/assets/6d8c3f29-4c9d-4947-b28f-0ff64e55e189)

![bazzite-steamos-steamdeck-OBS-interface-discover-OBS-store-notigv](https://github.com/user-attachments/assets/c75f47b7-eaf8-4682-84ae-c9430a35b81b)

*(Alternatively, open Konsole and type this command):*

![bazzite-steamos-steamdeck-OBS-interface-konsole-notigv](https://github.com/user-attachments/assets/f699ba28-3b43-4594-b5df-bd1c59330811)

![bazzite-steamos-steamdeck-OBS-interface-konsole-interface-notigv](https://github.com/user-attachments/assets/c5b1b277-4f9a-42d6-9361-ab6a231aa50e)

![bazzite-steamos-steamdeck-OBS-interface-konsole-interface-flathub-notigv](https://github.com/user-attachments/assets/3ae9ac93-b251-4cf8-b02d-fe7317a76b24)

```bash
flatpak install flathub com.obsproject.Studio
```

### Step 2: Install the OBS VkCapture Plugin
For OBS to see your games inside Game Mode, we need to install a bridge (plugin). Sometimes it doesn't show up in Discover, so the terminal is the fastest way! :D

Open your terminal (Konsole), paste this command and press Enter:

![bazzite-steamos-steamdeck-OBS-interface-konsole-notigv](https://github.com/user-attachments/assets/cb65d55c-6e5b-4348-a285-485172db689a)

![bazzite-steamos-steamdeck-OBS-interface-konsole-command-notigv](https://github.com/user-attachments/assets/7c3cbb77-3be1-4e88-9c59-525acfe5c09e)

```bash
flatpak install flathub com.obsproject.Studio.Plugin.OBSVkCapture
```
*Note: If it asks whether to install as "User" or "System", always choose **System**.*

### Step 3: The Emulator Fix (EmuDeck / Flatpak Users)
If you use emulators like Dolphin, RetroArch, or DuckStation installed via EmuDeck or Discover, they live inside a Flatpak "sandbox" that blocks OBS from seeing the video. We need to give them permission by installing a specific capture layer.

Open your terminal (Konsole)

![bazzite-steamos-steamdeck-OBS-interface-konsole-notigv](https://github.com/user-attachments/assets/ae303341-bd2c-4d55-b4cc-fc8aa2c45f4c)

Paste this command and press Enter:
```bash
flatpak install flathub org.freedesktop.Platform.VulkanLayer.OBSVkCapture
```
If the terminal gives you a numbered list of versions (like 21.08, 24.08, 25.08...), type the number for the **highest/newest version** (for example, type `5`) and press Enter. Press `Y` to confirm the installation.

![bazzite-steamos-steamdeck-OBS-interface-konsole-command-VK⁄GL-notigv](https://github.com/user-attachments/assets/ebb9b0a4-6ee6-4239-8e85-b9b852a7cfef)

* **Tip for Emulators:** Make sure your emulator's Video Backend / API is set to **Vulkan** in its graphical settings, otherwise the capture plugin might not detect it!

Done! The magic is installed. :D

---

## ⚙️ Configuring OBS
Open OBS Studio. Now we need to add the correct source and tweak a few things to avoid cropping or a giant zoom on your screen.

1. In the Sources box, click the **+** button.

![bazzite-steamos-steamdeck-OBS-interface-source-notigv](https://github.com/user-attachments/assets/5cebfc05-9a9a-4f87-bd1f-2153d995786e)

2. Select **Game Capture**. *(This option appears thanks to the plugin we just installed! :D)*

![bazzite-steamos-steamdeck-OBS-interface-source-options-notigv](https://github.com/user-attachments/assets/0feacf27-74b0-42f5-9169-7f9908fba0d2)

3. Right-click that source in the list -> **Transform** -> **Fit to screen**.

![bazzite-steamos-steamdeck-OBS-interface-source-notigv](https://github.com/user-attachments/assets/3c0bbf2e-42f7-4b47-be80-24b04dad4b7e)

![bazzite-steamos-steamdeck-OBS-interface-source-options-fit-notigv](https://github.com/user-attachments/assets/defa287f-7c3e-4078-a2d2-57c2a8c3dd86)

![bazzite-steamos-steamdeck-OBS-interface-source-options-fitscreen-notigv](https://github.com/user-attachments/assets/c8a7fdc7-5e39-4bd2-919b-5c48e37e72bb)

### 🖥️ For Ultrawide Users (21:9)
If you play on an Ultrawide monitor (like 3440x1440), OBS might crop your image if the canvas and output aren't set properly. Let's fix that! :D

1. Go to **Settings** -> **Video**. Change both Base (Canvas) Resolution and Output (Scaled) Resolution to `3440x1440`.

![bazzite-steamos-steamdeck-OBS-interface-source-options-ultrawide-notigv](https://github.com/user-attachments/assets/b218da79-6902-450c-875c-a5a5d849643b)

![bazzite-steamos-steamdeck-OBS-interface-source-options-ultrawide-video-notigv](https://github.com/user-attachments/assets/b3682438-d92a-4c1e-8345-263073af36dc)

2. Go to **Settings** -> **Output** -> **Recording**.

![bazzite-steamos-steamdeck-OBS-interface-source-options-ultrawide-notigv](https://github.com/user-attachments/assets/f9d53698-f911-4ccd-9333-23acb50c3bf9)

![bazzite-steamos-steamdeck-OBS-interface-source-options-ultrawide-output-notigv](https://github.com/user-attachments/assets/4c450caf-f2ed-489f-adde-c8f39afc0b52)

3. **¡IMPORTANT!** Make sure the **Rescale Output** option is Disabled. If it's checked, it will ruin your 21:9 aspect ratio! :(

![bazzite-steamos-steamdeck-OBS-interface-source-options-ultrawide-resolution-notigv](https://github.com/user-attachments/assets/36efcad2-e32b-4fbf-99e6-87227001b6e7)

4. Use the **Hybrid MP4** format so your videos won't corrupt if the power goes out.

![bazzite-steamos-steamdeck-OBS-interface-source-options-ultrawide-format-notigv](https://github.com/user-attachments/assets/289a85c5-be46-43ac-ada1-731dc030ee05)

6. In Video Encoder, select **FFmpeg VAAPI AV1** (if you have an AMD card that supports it) for better quality at half the file size.

![bazzite-steamos-steamdeck-OBS-interface-source-options-ultrawide-encoder-notigv](https://github.com/user-attachments/assets/f83e569f-602d-4dad-9781-492e0fec3a53)

---

## 🚀 Launch Options
To make the game send its image to OBS, we have to tell Steam to do so. Go to your Steam Library, right-click the game -> **Properties** -> **General** -> **Launch Options**.

![bazzite-steamos-steamdeck-OBS-launch-options-notigv](https://github.com/user-attachments/assets/8bcc1ced-2882-45ff-ac83-25f0089c7901)

![bazzite-steamos-steamdeck-OBS-launch-options-properties-notigv](https://github.com/user-attachments/assets/1d294636-5f46-4b00-9e7a-122324452066)

![bazzite-steamos-steamdeck-OBS-launch-options-general-notigv](https://github.com/user-attachments/assets/9e62d54b-5d08-4dcb-aedc-e49206221032)

Depending on what you are trying to play, follow the rule that applies to you:

**Case 1: The box is completely empty**
This applies to almost all native Steam games (like Hollow Knight) and clean emulators (like PPSSPP or Ryujinx). Just paste this:
```bash
OBS_VKCAPTURE=1 %command%
```
![bazzite-steamos-steamdeck-OBS-launch-options-case1-notigv](https://github.com/user-attachments/assets/afaf3183-f56b-4853-8943-57777d7e0a3d)

**Case 2: The box already has %command% in it**
If you already have environment variables (like `vblank_mode=0 %command%` for Dolphin), don't delete them! Just put our command at the very beginning and leave a space:
```bash
OBS_VKCAPTURE=1 vblank_mode=0 %command%
```

![bazzite-steamos-steamdeck-OBS-launch-options-case2-notigv](https://github.com/user-attachments/assets/a6716273-a269-4d0f-ac11-64af293bb98c)

![bazzite-steamos-steamdeck-OBS-launch-options-case2-solution-notigv](https://github.com/user-attachments/assets/42a8f18d-09c4-42a4-9ba8-c82a68e1241a)

**Case 3: The box has text, but NO %command%**
Very common in PCSX2 setups (e.g., `-fullscreen -batch`). Put our command AND the `%command%` variable at the very beginning, leaving a space before the original text:
```bash
OBS_VKCAPTURE=1 %command% -fullscreen -batch
```
![bazzite-steamos-steamdeck-OBS-launch-options-case3-notigv](https://github.com/user-attachments/assets/ce5530fe-2edb-478f-a080-71bc512fbeb3)

![bazzite-steamos-steamdeck-OBS-launch-options-case3-solution-notigv](https://github.com/user-attachments/assets/cbba327e-f76f-4bd1-95c7-2e91801f6d31)

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
