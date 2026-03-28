![PVZ GE-Gardenless-notigv-bazzite-Plants vs Zombies](https://github.com/user-attachments/assets/b2a21c17-0ba9-4684-92e7-11ecd5f2aac6)

# PvZ Gardendless on Steam Deck / Bazzite
**By NotiGV**

A fast, no-nonsense guide to playing the amazing PvZ Gardenless PC port directly from your Steam Library. Say goodbye to the missing WebView2 errors and black screens! :D

**Includes:**
* Downloading and safely organizing the game files.
* Adding the game to your Steam Library.
* The "Switcharoo" trick to install the required Microsoft WebView2 Runtime inside Proton.
* Installing GE-Proton to fix the black screen issues.

Let's plant some peashooters!! :D

---

## 📥 Step 1: Download & Organize
Since this is a standalone Windows port, we need to download it and put it in a safe place.

1. Go to Desktop Mode.
2. Open your browser and go to the official site: **[PvZ Gardendless (pvzge.com)](https://pvzge.com/en/)**

![NotiGV-PVZGE-Official site](https://github.com/user-attachments/assets/a0c603fc-21e6-4602-bf63-db7027d7d348)

3. Download the PC version *(it will likely be a .zip or .rar file)*.

![NotiGV-PVZGE-Official site-download](https://github.com/user-attachments/assets/7c51a698-a600-47d0-a75f-8091e2289f04)

![NotiGV-PVZGE-Official site-download-page](https://github.com/user-attachments/assets/c0ed4fd1-471d-4255-8874-fa51b3d0cfbc)

![NotiGV-PVZGE-Official site-download-page-Windows Platform](https://github.com/user-attachments/assets/3884d55c-cda6-4e2f-b77f-3ce82a13aa74)

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
Now we need to tell Steam where the game is.

1. Open Steam *(stay in Desktop Mode)*.

![NotiGV-PVZGE-Steam-Non game](https://github.com/user-attachments/assets/3e6fa967-9750-4e7d-a2be-f35a45362baa)

2. Click **Add a Game** at the bottom left -> **Add a Non-Steam Game...**

![NotiGV-PVZGE-Steam-Non game 2](https://github.com/user-attachments/assets/d98503b4-605d-40b0-b20b-af64aef4f3f7)

![NotiGV-PVZGE-Steam-Non game 3](https://github.com/user-attachments/assets/0b703f17-01b6-48a6-8ed5-d434dc72403d)

3. Click the **Browse...** button.

![NotiGV-PVZGE-Steam-Non game 4](https://github.com/user-attachments/assets/1a349717-dd7f-4de2-8f2f-d1997934571e)

4. Navigate to your safe folder (`~/Games/PvZ_Gardendless`).

![NotiGV-PVZGE-file-folder](https://github.com/user-attachments/assets/b548d93d-b97b-431d-8dac-41208d355b68)

   * *Note: Make sure to change the file type filter at the bottom to "All Files" if you don't see the game!*
   
5. Select the game's main `.exe` file and click **Open**.

![NotiGV-PVZGE-file](https://github.com/user-attachments/assets/b20379cd-358c-422c-85ea-180276c6fa1f)

6. Click **Add Selected Programs**.

---

## 🔀 Step 3: The WebView2 Fix (The Switcharoo Trick)
If you try to run the game now, you will get an error saying: *"Could not find the WebView2 Runtime"*. 
Because we are using Proton (Linux), the game doesn't have access to this Windows/Edge component. Here is the trick to install it inside the game's sandbox:

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
6. Click **Browse...** right below it, and select the **WebView2 Installer** you just downloaded.

![NotiGV-PVZGE-Steam-properties 3](https://github.com/user-attachments/assets/55f6095a-4ba5-4109-ab2c-e83259c309a7)

![NotiGV-PVZGE-Steam-properties 3 5](https://github.com/user-attachments/assets/ce9cabf2-66b7-4683-9a5d-1ef051e9ee9c)

7. Close the properties window and click the green **Play** button in Steam.

![NotiGV-PVZGE-Steam-properties 4](https://github.com/user-attachments/assets/a4a160ef-40ca-4df6-929b-67d696326c53)

8. This will run the Microsoft Installer inside the game's Proton prefix! Follow the on-screen steps to install it :D

![NotiGV-PVZGE](https://github.com/user-attachments/assets/2b4fb11c-e66a-4f81-8a8c-9e13f3cb1129)

9. Once it finishes and closes, go back to the game's Properties. **Delete** the installer path from the Target field, and **Paste your original game path** back in.

![NotiGV-PVZGE-Steam-properties](https://github.com/user-attachments/assets/8c53aee1-128e-40b3-9b31-508ee5ad4b61)

![NotiGV-PVZGE-Steam-properties 3 5](https://github.com/user-attachments/assets/e5439b41-06e3-486d-afd7-a883d357493a)

![NotiGV-PVZGE-Steam-properties 2](https://github.com/user-attachments/assets/dfd1190f-820d-4b3c-a209-fe125da36021)

---

## 🖤 Step 4: Fixing the Black Screen (GE-Proton)
The game now has the web engine it needs, but standard Proton might give you a completely black screen. We need a custom community version called GE-Proton :D

![NotiGV-PVZGE-Black Screen](https://github.com/user-attachments/assets/b83b1646-c1ab-480a-b73f-d01b8e4415a0)

1. Open the Discover Store (the shopping icon).

![NotiGV-PVZGE-Bazaar](https://github.com/user-attachments/assets/bdb2fbaa-ee03-427e-839e-63bdf2c6c365)

2. Search for **ProtonUp-Qt** and click Install.

![NotiGV-PVZGE-Bazaar-ProtonUP](https://github.com/user-attachments/assets/65926b58-24bb-407a-af0a-795043b973a0)

3. Open ProtonUp-Qt and click **Add version**.

![NotiGV-PVZGE-Bazaar-ProtonUP-open](https://github.com/user-attachments/assets/589f82cb-f3c2-496a-9a35-f6b971cde5c6)

![NotiGV-PVZGE-Bazaar-ProtonUP-open 2](https://github.com/user-attachments/assets/68217189-b8e7-4743-9767-a28b74978e29)

![NotiGV-PVZGE-Bazaar-ProtonUP-add version](https://github.com/user-attachments/assets/425d6a6a-d7ae-41ec-a4ff-c37991df7c31)

4. Make sure the Compatibility tool is set to **GE-Proton**, select the latest version (like `GE-Proton9-XX`), and click **Install**.

![NotiGV-PVZGE-Bazaar-ProtonUP-add version 2](https://github.com/user-attachments/assets/fbcc300b-b2a8-4acf-ae15-d633876115a8)

5. **IMPORTANT:** Completely close Steam *(Right-click the Steam icon in your taskbar -> Exit)* and open it again so it detects the new tool.

![NotiGV-PVZGE-Steam-Exite](https://github.com/user-attachments/assets/10f800ea-07de-4255-93ac-dec669ab0f07)

---

## ✨ Step 5: Final Polish & Game Mode
We are almost done!

1. Go to the **Properties** of your game in Steam.

![NotiGV-PVZGE-Steam-properties](https://github.com/user-attachments/assets/6cdc53f2-6676-4e53-8300-a755ecc2d1fe)

2. Go to the **Compatibility** tab.

![NotiGV-PVZGE-Steam-Properties 5](https://github.com/user-attachments/assets/b49cbb8f-a43d-4baa-b996-47bd0bb54a73)

3. Check the box for **Force the use of a specific Steam Play compatibility tool**.

![NotiGV-PVZGE-Steam-Properties 6](https://github.com/user-attachments/assets/0a7cdd96-d864-442b-b802-0261368ba2c7)

4. Select the **GE-Proton** version you just installed from the dropdown menu.

![NotiGV-PVZGE-Steam-Properties 5](https://github.com/user-attachments/assets/203ead9f-00a3-449c-bee0-bb18be0d944f)

5. Switch back to Game Mode.
6. Launch the game! It will now load perfectly. :D

![NotiGV-PVZGE-ingame](https://github.com/user-attachments/assets/c611f747-3924-4102-87de-242e9dabfd72)


*Note for Ultrawide Users: Since this game was designed for traditional aspect ratios, you will see black bars on the sides if you play on a 21:9 monitor. This is completely normal! On a handheld, it will fill the screen perfectly :D*

---

## 📝 Author's Note :D
Setting up web-based fan games on Linux can be a little tricky with the WebView2 requirements, but the "Switcharoo" trick is a lifesaver you can use for many other games too!

I highly recommend right-clicking the empty game icon in your Steam Library and adding some custom artwork (Grid, Hero, and Logo) from SteamGridDB to make it look official.

![NotiGV-PVZGE-ingame 2](https://github.com/user-attachments/assets/3ab9ce4c-3272-497a-a295-27f65afa0f87)

Have fun defending your garden! Let me know in the comments if this worked for you! :D
---

## 📖 Read the Full Guide
If you prefer to read this guide with rich formatting, see the step-by-step screenshots, or want to drop a comment to the community, check out the official Steam version right here:

👉 **[Read and Favorite the Official Steam Guide Here](https://steamcommunity.com/sharedfiles/filedetails/?id=3693050959)**

---

>
>***Disclaimer & Credits:*** This technical guide was written and formatted by NotiGV for educational purposes and to help the Linux and handheld gaming community troubleshoot compatibility issues.
>
>***Asset & Property Rights:*** PvZ Gardendless is a fan-made project. All original Plants vs. Zombies assets, characters, and intellectual properties belong to PopCap Games and Electronic Arts (EA). This guide does not host, provide, or directly distribute the game files or Microsoft binaries. All links point to the official project page and Microsoft's official developer resources.
>
>***Editing Process:*** Digital creation and language assistance tools were utilized during the final proofreading of this guide to ensure clear, concise, and accurate technical instructions.

*Happy gaming! :D*
