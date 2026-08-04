![PVZ GE-Gardenless-notigv-bazzite-Plants vs Zombies](https://github.com/user-attachments/assets/b2a21c17-0ba9-4684-92e7-11ecd5f2aac6)

# PvZ Gardendless on Steam Deck / Bazzite
**By ThatGVguy**

A fast, no-nonsense guide to playing the amazing PvZ Gardenless PC port directly from your Steam Library. Say goodbye to the missing WebView2 errors and black screens! :D

The whole point of this guide is so anyone can join this awesome community without breaking thier head trying to figure out Linux prefixes and weird terminal commands. So... grab a Taco and let's plant some peashooters!! :D

**Includes:**
* Downloading and safely organizing the game files.
* Adding the game to your Steam Library.
* The "Switcharoo" trick to install the required Microsoft WebView2 Runtime inside Proton.
* Installing GE-Proton to fix the black screen issues.

---

## 📥 Step 1: Download & Organize
First things first! Since this is a standalone Windows port, we need to download it and put it in a safe place.

1. Go to Desktop Mode.
2. Open your trusty web browser and go to the official site: **[PvZ Gardendless (pvzge.com)](https://pvzge.com/en/)**

<img width="2547" height="1289" alt="ThatGVguy-PVZGE-Official site" src="https://github.com/user-attachments/assets/88550d39-4809-4bb9-9606-f47fe7cd8ea2" />

3. Download the PC version *(it will likely be a .zip or .rar file)*.

<img width="252" height="118" alt="ThatGVguy-PVZGE-Official site-download" src="https://github.com/user-attachments/assets/90b20c10-5ced-4640-b096-dbb50075a839" />
<img width="1264" height="872" alt="ThatGVguy-PVZGE-Official site-download-page" src="https://github.com/user-attachments/assets/b1df65ef-147e-4a76-99c9-8d49f7284069" />
<img width="340" height="227" alt="ThatGVguy-PVZGE-Official site-Platform-page" src="https://github.com/user-attachments/assets/21d860c2-097b-4c13-bd15-4fa970dc5d67" />
<img width="1225" height="527" alt="ThatGVguy-PVZGE-Official site-download-page-Windows Platform" src="https://github.com/user-attachments/assets/9d2d2082-9d0b-4806-8726-b87358e2311f" />

4. Open your File Manager (Dolphin) and go to your **Downloads** folder.

   ![NotiGV-PVZGE-Dolphin](https://github.com/user-attachments/assets/8dd55501-2207-4a4a-b8f6-95fa4d60a913)
   ![NotiGV-PVZGE-file zip](https://github.com/user-attachments/assets/93c84334-140b-4531-81c0-7582ae49832e)
   ![NotiGV-PVZGE-file zip-extract](https://github.com/user-attachments/assets/0504a17e-66fd-45b1-89fe-a34a7c2c20c3)
   ![NotiGV-PVZGE-file](https://github.com/user-attachments/assets/8331bb13-4ea9-4a30-bb69-29ba2802e597)

5. Extract the contents of the downloaded file.
6. Create a safe, permanent folder for it. *(For example, create a `Games` folder inside your Home directory: `~/Games/PvZ_Gardendless`)*.

   ![NotiGV-PVZGE-file-folder](https://github.com/user-attachments/assets/069e27d3-5380-48a5-a73d-a415480ead0f)
   ![NotiGV-PVZGE-file-folder-inside](https://github.com/user-attachments/assets/060c1297-ca54-4263-b610-39b312231f6b)

7. Move the extracted game files there. Do not leave it in Downloads, or you might accidentally delete it later! :D

---

## 🎮 Step 2: Add to Steam
Now we need to tell Steam where the game actully is.

1. Open Steam *(stay in Desktop Mode)*.

   ![NotiGV-PVZGE-Steam-Non game](https://github.com/user-attachments/assets/3e6fa967-9750-4e7d-a2be-f35a45362baa)

2. Click **Add a Game** at the bottom left -> **Add a Non-Steam Game...**

   ![NotiGV-PVZGE-Steam-Non game 2](https://github.com/user-attachments/assets/d98503b4-605d-40b0-b20b-af64aef4f3f7)
   ![NotiGV-PVZGE-Steam-Non game 3](https://github.com/user-attachments/assets/0b703f17-01b6-48a6-8ed5-d434dc72403d)

3. Click the **Browse...** button.

   ![NotiGV-PVZGE-Steam-Non game 4](https://github.com/user-attachments/assets/1a349717-dd7f-4de2-8f2f-d1997934571e)

4. Navigate to your safe folder (`~/Games/PvZ_Gardendless`).

   ![NotiGV-PVZGE-file-folder](https://github.com/user-attachments/assets/b548d93d-b97b-431d-8dac-41208d355b68)

   > *Note: Make sure to change the file type filter at the bottom to "All Files" if you don't see the game!*
   
5. Select the game's main `.exe` file and click **Open**.

   ![NotiGV-PVZGE-file](https://github.com/user-attachments/assets/b20379cd-358c-422c-85ea-180276c6fa1f)

6. Click **Add Selected Programs**.

---

## 🔀 Step 3: The WebView2 Fix (The Switcharoo Trick)
Listen up, because this is where the magic happens! If you try to run the game now, you will get an error saying: *"Could not find the WebView2 Runtime"*. 

Because we are using Proton (Linux), the game doesn't have access to this Windows/Edge component out of the box. And if you just add the installer as a separate Non-Steam game, Steam creates a brand new isolated folder so they cant see each other. Here is the trick to install it inside the game's sandbox:

![NotiGV-PVZGE-WebView2](https://github.com/user-attachments/assets/556cf7e5-18f1-4f24-9d38-a18f973cd534)

1. Go to the official Microsoft download page: **[Microsoft Edge WebView2](https://developer.microsoft.com/en-us/microsoft-edge/webview2/?form=MA13LH)**

   ![NotiGV-PVZGE-WebView2 site](https://github.com/user-attachments/assets/846c52ce-2144-4d23-a702-6d8590eaff7b)

2. Scroll down to the **Evergreen Standalone Installer** section and download the **x64** version.

   ![NotiGV-PVZGE-WebView2 site- download](https://github.com/user-attachments/assets/bd688288-2ffd-4106-a820-731bac151a40)
   ![NotiGV-PVZGE-WebView2 site- download 2](https://github.com/user-attachments/assets/78e26a65-c518-4aa7-b6b5-baf1f6aa019c)
   ![NotiGV-PVZGE-WebView2 site- download 3](https://github.com/user-attachments/assets/af12acdc-943a-4dfc-8024-7f35b6208b7f)

3. Save that `.exe` installer inside your `PvZ_Gardendless` game folder so it's easy to find.

   ![NotiGV-PVZGE-file-folder-inside](https://github.com/user-attachments/assets/dfeee411-cb3c-4174-be5d-39193d708b93)

4. Go to your Steam Library, find your newly added PvZ Gardendless shortcut, right-click it -> **Properties**.

   ![NotiGV-PVZGE-Steam-properties](https://github.com/user-attachments/assets/1c4a4414-ef5f-4376-8b0b-092decc4854f)
   ![NotiGV-PVZGE-Steam-properties 2](https://github.com/user-attachments/assets/9628516f-1ba8-4830-9097-a27fc16c6cb3)

5. In the Shortcut tab, look at the **Target** field. **Copy that entire path** and paste it somewhere safe (like a blank text document). We will need it back in a minute! 

   > **IMPORTANT:** If your path has quotes `""` around it, make sure to copy them too! If your folder has a space in it, Steam requires those quotes or it completly breaks the path!

6. Click **Browse...** right below it, and select the **WebView2 Installer** you just downloaded.

   ![NotiGV-PVZGE-Steam-properties 3](https://github.com/user-attachments/assets/55f6095a-4ba5-4109-ab2c-e83259c309a7)
   ![NotiGV-PVZGE-Steam-properties 3 5](https://github.com/user-attachments/assets/ce9cabf2-66b7-4683-9a5d-1ef051e9ee9c)

7. **CRITICAL STEP:** Go to the **Compatibilty** tab and check **"Force the use of a specific Steam Play compatibility tool"**. Select **Proton Experimental** (or GE-Proton). If you skip this, the installer will just open and close immediatly!

8. Close the properties window and click the green **Play** button in Steam.

   ![NotiGV-PVZGE-Steam-properties 4](https://github.com/user-attachments/assets/a4a160ef-40ca-4df6-929b-67d696326c53)

9. This will run the Microsoft Installer inside the game's Proton prefix! Follow the on-screen steps to install it :D

   ![NotiGV-PVZGE](https://github.com/user-attachments/assets/2b4fb11c-e66a-4f81-8a8c-9e13f3cb1129)

10. Once it finishes and closes, go back to the game's Properties. **Delete** the installer path from the Target field, and **Paste your original game path** back in. **(Make sure to include the quotes `""` around the path if it had them!)**

    ![NotiGV-PVZGE-Steam-properties](https://github.com/user-attachments/assets/8c53aee1-128e-40b3-9b31-508ee5ad4b61)
    ![NotiGV-PVZGE-Steam-properties 3 5](https://github.com/user-attachments/assets/e5439b41-06e3-486d-afd7-a883d357493a)
    ![NotiGV-PVZGE-Steam-properties 2](https://github.com/user-attachments/assets/dfd1190f-820d-4b3c-a209-fe125da36021)

---

## 🖤 Step 4: Fixing the Black Screen (GE-Proton)
The game now has the web engine it needs, but standard Proton might give you a completly black screen. We need a custom community version called GE-Proton to fix it :D

![NotiGV-PVZGE-Black Screen](https://github.com/user-attachments/assets/b83b1646-c1ab-480a-b73f-d01b8e4415a0)

1. Open the Discover Store (the shopping icon).

   ![NotiGV-PVZGE-Bazaar](https://github.com/user-attachments/assets/bdb2fbaa-ee03-427e-839e-63bdf2c6c365)

2. Search for **ProtonUp-Qt** and click Install.

   ![NotiGV-PVZGE-Bazaar-ProtonUP](https://github.com/user-attachments/assets/65926b58-24bb-407a-af0a-795043b973a0)

3. Open ProtonUp-Qt and click **Add version**.

   ![NotiGV-PVZGE-Bazaar-ProtonUP-open](https://github.com/user-attachments/assets/589f82cb-f3c2-496a-9a35-f6b971cde5c6)
   ![NotiGV-PVZGE-Bazaar-ProtonUP-open 2](https://github.com/user-attachments/assets/68217189-b8e7-4743-9767-a28b74978e29)
   ![NotiGV-PVZGE-Bazaar-ProtonUP-add version](https://github.com/user-attachments/assets/425d6a6a-d7ae-41ec-a4ff-c37991df7c31)

4. Make sure the Compatibility tool is set to **GE-Proton**, select the latest version (for example, `GE-Proton10-34` works amazing for me), and click **Install**.

   ![NotiGV-PVZGE-Bazaar-ProtonUP-add version 2](https://github.com/user-attachments/assets/fbcc300b-b2a8-4acf-ae15-d633876115a8)

5. **IMPORTANT:** Completely close Steam *(Right-click the Steam icon in your taskbar -> Exit)* and open it again so it detects the new tool.

   ![NotiGV-PVZGE-Steam-Exite](https://github.com/user-attachments/assets/10f800ea-07de-4255-93ac-dec669ab0f07)

---

## ✨ Step 5: Final Polish & Game Mode
We are almost done!

1. Go to the **Properties** of your game in Steam.

   ![NotiGV-PVZGE-Steam-properties](https://github.com/user-attachments/assets/6cdc53f2-6676-4e53-8300-a755ecc2d1fe)

2. Go to the **Compatibilty** tab.

   ![NotiGV-PVZGE-Steam-Properties 5](https://github.com/user-attachments/assets/b49cbb8f-a43d-4baa-b996-47bd0bb54a73)

3. Check the box for **Force the use of a specific Steam Play compatibility tool**.

   ![NotiGV-PVZGE-Steam-Properties 6](https://github.com/user-attachments/assets/0a7cdd96-d864-442b-b802-0261368ba2c7)

4. Select the **GE-Proton** version you just installed from the dropdown menu.

   ![NotiGV-PVZGE-Steam-Properties 5](https://github.com/user-attachments/assets/203ead9f-00a3-449c-bee0-bb18be0d944f)

5. Switch back to Game Mode.
6. Launch the game! It will now load perfectly. :D

   ![NotiGV-PVZGE-ingame](https://github.com/user-attachments/assets/c611f747-3924-4102-87de-242e9dabfd72)

> **Note for Ultrawide Users:** Since this game was designed for traditional aspect ratios, you will see black bars on the sides if you play on a 21:9 monitor like I do on my desktop PC. This is completly normal! But on a handheld device, it will fill the screen perfectly :D

---

## 🦦 Plan B: The Lutris Alternative (If Steam is Stubborn) :( (SteamDeck Users)
Sometimes, Steam just flat out refuses to cooperate with specific webview setups depending on your OS, leaving you stuck in an infinite black or white screen loop. 

**A MASSIVE shoutout to community member Glizzy Grizzy and zero from Discord!** They actualy figured out that while this works out of the box on Bazzite, SteamOS users specifically need a custom runner called **Proton CachyOS** via Lutris to make WebView2 behave! :D

Lutris handles Windows prefixes a little differently, making it a lifesaver for weird ports like this. The process is almost the exact same, we just do the "Switcharoo" trick first!

1. Open the Discover Store in Desktop Mode, search for **Lutris** and install it if you haven't already.
2. Go to the official Microsoft download page and download the **Evergreen Standalone Installer (x64)** for **WebView2** and keep it handy.
![NotiGV-PVZGE-WebView2 site- download](https://github.com/user-attachments/assets/bd688288-2ffd-4106-a820-731bac151a40)
![NotiGV-PVZGE-WebView2 site- download 2](https://github.com/user-attachments/assets/78e26a65-c518-4aa7-b6b5-baf1f6aa019c)
![NotiGV-PVZGE-WebView2 site- download 3](https://github.com/user-attachments/assets/af12acdc-943a-4dfc-8024-7f35b6208b7f)

3. Now, open **ProtonUp-Qt** (install it from Discover if you don't have it).

![NotiGV-PVZGE-Bazaar](https://github.com/user-attachments/assets/bdb2fbaa-ee03-427e-839e-63bdf2c6c365)
![NotiGV-PVZGE-Bazaar-ProtonUP-open](https://github.com/user-attachments/assets/589f82cb-f3c2-496a-9a35-f6b971cde5c6)

Under "Install for", click the dropdown arrow and change it to **Lutris Flatpak** (or just Lutris).

<img width="551" height="487" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-Proton-thatgvguy" src="https://github.com/user-attachments/assets/77dcd4d3-7925-4642-b178-0b98b9f92ab0" />
<img width="551" height="487" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-Proton 2-thatgvguy" src="https://github.com/user-attachments/assets/d804e41f-ab2a-48e3-a2ad-8d9709393bcc" />

Click **Add version**, change the compatibility tool to **proton-cachyos** (it's probly the default one that shows up), and hit Install.

<img width="551" height="487" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-Proton 3-thatgvguy" src="https://github.com/user-attachments/assets/b0705354-b8b6-4835-87f5-92f430cc4e6e" />
<img width="551" height="487" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-Proton 4-thatgvguy" src="https://github.com/user-attachments/assets/0c40e3b6-2f61-406e-88e5-7703517b7e4d" />

4. Open Lutris and click the **"+"** button in the top left corner to add a new game. Select **"Add locally installed game"**.

### <img width="1519" height="809" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy" src="https://github.com/user-attachments/assets/1181bfd0-0894-435b-9e54-3d913fe9026a" />

### <img width="58" height="56" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 2" src="https://github.com/user-attachments/assets/228f932d-e23e-4c62-bad8-b69f19af90f9" />

### <img width="791" height="614" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 3" src="https://github.com/user-attachments/assets/e549638f-b794-45f4-b3c8-afc7908de563" />

5. Name it *PvZ Gardenless*.

<img width="1046" height="701" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 4" src="https://github.com/user-attachments/assets/d46de342-d1c9-4a05-9af1-544a4126a4ed" />

6. Go to the **Game options** tab. For the **Executable**, click browse and point it to the **WebView2 Installer** `.exe` you downloaded.

<img width="1046" height="701" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 5" src="https://github.com/user-attachments/assets/a3f0c751-ff5c-47f7-a0de-60c54771fd3d" />

<img width="1490" height="336" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 6" src="https://github.com/user-attachments/assets/698e3395-1321-4160-b05f-e2f08515c1a4" />

7. **THE MAGIC FIX:** Go to **Configure -> Runner options**, and make sure your Wine version is set to the **CachyOS** version you just installed. This is what prevents the SteamOS white screen crash!

<img width="1048" height="656" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 7" src="https://github.com/user-attachments/assets/8b220ab1-b811-4413-9914-31d76a9da97d" />

8. Hit **Save**, then click the **Play** button in Lutris. It will actully run the Microsoft installer inside a fresh Wine prefix! Follow the prompts to finish the install.

<img width="1060" height="798" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 8" src="https://github.com/user-attachments/assets/e23d3d38-9b82-4109-9766-0eed7f87c7b7" />

<img width="1520" height="806" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 9" src="https://github.com/user-attachments/assets/3de99aa4-30d1-468f-9ae1-9ed957b3c343" />

9. Once it's done, right-click the game in Lutris and click **Configure**.

10. Go back to **Game options** and change the **Executable** path to your main `PvZ_Gardendless.exe` file.

<img width="1502" height="477" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 10" src="https://github.com/user-attachments/assets/1aa92244-8cdd-4e92-8d5a-1746ab7acee6" />

<img width="1049" height="722" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 11" src="https://github.com/user-attachments/assets/ccc06aa9-81cc-4736-b4ae-fc9c33fedfd0" />

<img width="994" height="786" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 12" src="https://github.com/user-attachments/assets/7739f9a6-cbdd-4c0c-9973-98b711721788" />

11. **Want it on Steam?** Right-click your game in Lutris and select **"Create Steam shortcut"**. If you don't see it appear in Steam right away, just close Steam completely and open it back up. Now you can play PvZ directly from your Steam Library in Game Mode! :D

*(Note: The game might close the very first time you launch it. Just reopen it and it should work perfectly!)*

<img width="634" height="741" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 13" src="https://github.com/user-attachments/assets/75720aad-4760-49b7-994f-974bdc9ee32c" />

<img width="3086" height="941" alt="PVZ-Gardendless-steam-deck-bazzite-lutrix-thatgvguy 14" src="https://github.com/user-attachments/assets/d6f52ffe-2d54-48e6-a984-43e7af495e61" />

Hit play and enjoy!! :D

---

## 📝 Author's Note :D
If you made it this far, your officially ready to defend your garden! Setting up web-based fan games on Linux can be a little tricky with the WebView2 requirements, but the "Switcharoo" trick is a lifesaver you can use for many other games too!

I highly recommend right-clicking the empty game icon in your Steam Library and adding some custom artwork (Grid, Hero, and Logo) from SteamGridDB to make it look official.

![NotiGV-PVZGE-ingame 2](https://github.com/user-attachments/assets/3ab9ce4c-3272-497a-a295-27f65afa0f87)

Have fun defending your garden! Let me know in the comments if this worked for you, or if you run into any weird errors. I'll answer you, or someone else from the community will drop in to help! :D

---

## 📖 Read the Full Guide
If you prefer to read this guide with rich formatting, see the step-by-step screenshots, or want to drop a comment to the community, check out the official Steam version right here:

👉 **[Read and Favorite the Official Steam Guide Here](https://steamcommunity.com/sharedfiles/filedetails/?id=3693050959)**

---

> **Disclaimer & Credits:** This technical guide was written and formatted by ThatGVguy for educational purposes and to help the Linux and handheld gaming community troubleshoot compatibility issues.
>
> **Asset & Property Rights:** PvZ Gardendless is a fan-made project. All original Plants vs. Zombies assets, characters, and intellectual properties belong to PopCap Games and Electronic Arts (EA). This guide does not host, provide, or directly distribute the game files or Microsoft binaries. All links point to the official project page and Microsoft's official developer resources.
>
> **Editing Process:** Digital creation and language assistance tools were utilized during the final proofreading of this guide to ensure clear, concise, and accurate technical instructions.
>
> Happy gaming! :D
> 
> \- **ThatGVguy** :D
