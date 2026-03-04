![flash-games-steam-deck-bazzite-gamemode-ruffle-notigv](https://github.com/user-attachments/assets/14fc865b-f7a6-4673-a850-5117ea698bc7)

# How to Play Classic Flash Games Natively on Steam Deck & Bazzite (Ruffle Guide)
**By NotiGV**

Preserve web classics like **Alien Hominid**, **Fancy Pants** and **Mario 63** directly in your Steam UI, no browser needed!

Hey everyone! :D
I just put together a quick guide on how to get classic Flash games running natively in the Steam UI using **Ruffle**. It works perfectly on Steam Deck and Bazzite (Fedora Atomic), and it’s a great way to preserve those web classics without needing complex scripts.

Here is the quick setup to get you gaming in minutes.

---

## ⚙️ The Quick Setup

### 1. Get the Emulator
First, we need the Ruffle emulator (Flatpak).
* Boot into **Desktop Mode**.
* Open the **Discover Store**.
* Search for and install **Ruffle**.

### 2. Get the Game
* Download your favorite `.swf` file (the Internet Archive is your friend here).
* Put it in a dedicated folder (e.g., `Documents/Flash Games`).
* **Important:** Right-click the `.swf` file and select **"Copy Location"**. We will need this path.

### 3. Add to Steam & Configure Launch Options
* Open Steam in Desktop Mode and click **“Add a Non-Steam Game”**.
* Select **Ruffle** from the list.
* Right-click Ruffle in your library -> **Properties** -> **Launch Options**.

**The Command:** Keep the default code that is already there, add a space at the very end, and paste your game path *inside quotes*. It should look exactly like this example:

```bash
"run" "--branch=stable" "--arch=x86_64" "--command=ruffle" "--file-forwarding" "rs.ruffle.Ruffle" "@@u" "@@" "/home/deck/Emulation/roms/Flash/Cactus McCoy.swf"
```

### 4. Controls (Steam Input)
Most Flash games rely on the keyboard (Arrow Keys + Space/Z/A).
* Once back in Gaming Mode, open the controller settings for your new Ruffle shortcut.
* Map your D-Pad to the Arrow Keys, and your face buttons to the required keyboard keys using **Steam Input**.

---

## 📖 Want the Full Step-by-Step?
I wrote a detailed guide on Steam Community with full screenshots, explaining how to **add multiple games** (since Ruffle disappears from the non-Steam game list after the first time) and extra troubleshooting tips.

👉 **[Read the Full Guide on Steam Here](https://steamcommunity.com/sharedfiles/filedetails/?id=3666492820)**

Let me know if you have any issues setting it up! :D

---

> ***Disclaimer:*** This technical guide was written and formatted by NotiGV to help the Linux and handheld gaming community optimize their emulation setups. The Flatpak commands provided are standard, safe system-level commands for Bazzite/SteamOS. Applying custom launch options is always done at your own discretion.
>   
> ***Editing Process:*** Digital creation and language assistance tools were utilized during the final proofreading of this guide to ensure clear, concise, and accurate technical instructions.
