<img width="800" height="800" alt="The Forest-ThatGVguy-bazzite" src="https://github.com/user-attachments/assets/3d50ee4e-fcaa-4cfd-bb2e-d749dbfc6a7c" />

# The Forest on Bazzite Desktop Linux: The Ultimate Performance & Setup Guide
**By ThatGVguy**

A fast, no-nonsense guide to getting The Forest running absolutely flawlessly on Bazzite Linux. Stop guessing with the settings menu and start surviving! The whole point of this guide is to help you get the best visual quality, eliminate blurry cinematic filters, and stop heavy "Ultra" settings from choking your CPU for no reason. 

So, grab your trusty axe, and let's get your game looking crisp! :D

**Includes:**
* The definitive In-Game settings for a sharp, high-FPS experince.
* SteamOS/Gamescope menu tweaks tailored for your desktop setup.
* Proton compatibility testing and the perfect launch commands to squeeze every drop of perfomance out of your AMD hardware.

Let's get into the woods!! :D

---

## 🖥️ The Test Rig (My Setup)
Just to give you an idea of the PC this is being tested on. Keep in mind your perfomance might change a lot depending on your specific components :D and monitor, but the Proton and Gamescope menu sections will totally work for you anyway! :D

**The Desktop Rig (Ultrawide Gaming & Streaming)**
* **OS:** Bazzite
<img width="960" height="960" alt="Bazzite_Logo-ThatGVguy" src="https://github.com/user-attachments/assets/d163786e-c5d7-458c-b026-e3c8afaa79b3" />
* **CPU:** AMD Ryzen 5 5600
<img width="800" height="800" alt="AMD Ryzen 5 5600" src="https://github.com/user-attachments/assets/3d3bb854-19e6-4ed9-9e53-9770980fbaae" />
* **GPU:** ASRock Challenger Radeon RX 7800 XT OC (16GB VRAM)
<img width="800" height="500" alt="DUALFANDESIGN-Radeon RX 7800 XT Challenger 16GB OC_mobile" src="https://github.com/user-attachments/assets/8e2d7b3f-c18d-46c6-8024-21abb262e3a2" />
* **RAM:** 16 GB (2x8) T-Force Delta R @ 3200MHz
<img width="1000" height="1000" alt="16 GB (2x8) T-Force Delta R @ 3200MHz" src="https://github.com/user-attachments/assets/4bf406a5-492b-44d6-bd5f-1f49c96788bb" />
* **Monitor:** Xiaomi G34WQi (Ultrawide 21:9, 1440p, 180Hz)
<img width="1600" height="1600" alt="_Xiaomi G34WQi" src="https://github.com/user-attachments/assets/c39f4439-155b-498e-b825-44a478ea7dea" />

---

## 🌲 In-Game Settings (The Sweet Spot)
*This setup maintains maximum visual quality while eliminating those annoying blurry cinematic filters. It also reduces a few "Ultra" options that bottleneck your CPU without giving you any real visual benefit.*

### Left Column Settings
* **Antialiasing:** `HIGH (TAA)`
* **Shadows:** `HIGH` (Avoid *Very High*, it consumes way too many resources for a difference you will barely even notice. Trustme I cant tell the difference :().
* **Far Shadows:** `ON`.
* **Draw Distance:** `HIGH` or `VERY HIGH` (If your GPU can handle this with zero sweat, but **High** is usually more than enough)
* **Sunshine Occlusion:** `ON`.
* **Light Scatter:** `HIGH`.
* **Terrain:** `PARALLAX` (Makes the mud and rocks look super 3D and awesome!!).
* **Texture Quality:** `FULL RESOLUTION` (You paid for that VRAM, let's use it all! :D).
* **Grass Distance:** `FAR`. If you want it on **Very FAR** you will see more grass in the distance, but that really depends on whether you prefer it or not, In my case, I don't see it neccesary at all ;)
* **Grass Density:** `HIGH` (Lowering this from **Ultra** to **High** is an absolute lifesaver. It takes a massive load off your CPU and definetly improves your 1% lows).

### Right Column Settings
**(Quick note here: You can honestly set most of these to Ultra, but to be honest there isn't much of a difference in my opinion, so save those frames for smoother gameplay!)**

* **Ocean Quality:** `LOW`. This one is dynamic! If you go to the ocean a lot or live there and want to see as best as possible underwater, **Flat** is without a doubt the best option (the water gets way more transparent). But if you want a realistic experience, **Low** and **High** are fine. I personally keep it on *Low* because I almost never visit the ocean anyway :D
* **SSAO Type:** `AMPLIFY`.
* **SSAO Quality:** `HIGH` (Stay away from **Ultra** here, trustme it eats frames for breakfast)
* **Motion Blur:** `OFF` **(CRITICAL!)** (When you are pushing high frames, this literally just smears your screen).
* **Chromatic Aberration:** `OFF` **(CRITICAL!)** (Turns off that weird color distortion on the edges of the screen for a much cleaner look) :)
* **Bloom:** `ON`.
* **Film Grain:** `OFF` **(CRITICAL!)** (Removes that visual "noise" so you can see the forest in crystal clear HD)
* **Color Grading:** `ORIGINAL` (Or whatever you personally prefer)
* **Screen Space Reflection:** `ON`.
* **Volumetric Clouds:** `ON`. If you want to see wispy clouds

---

## ⚙️ Steam / Gamescope Configuration (Bazzite Side Menu)

**💡 Quick Tip:** When you launch the game, you might see a small Steam window popping up saying it's processing Vulkan shaders. Just let it finish! It takes 10 seconds at most, and your in game perfomance will seriously thank you later! :b 

*These are the tweaks you apply in the quick access performance menu (the one you open with the three-dot button or Home button + A on Xbox Layout/ X on Playstation / B on Switch).*

* **Frame Limit:** Set this about **5 to 8 FPS below your monitor's maximum**. Why? Because if you hit your absolute max refresh rate, you step outside your VRR/FreeSync window and V-Sync forces itself on, giving you annoying input lag. Capping it just below the limit keeps everything buttery smooth and responsive!
* **Enable VRR (FreeSync):** **ON** (This makes sure your monitor syncs perfectly with your FPS so you don't feel any stutters).
* **Enable HDR:** **OFF** (The game just doesn't support it natively).
* **Allow Tearing:** **OFF** (Since we have VRR active, leaving this on would just cause unnecesary visual tearing).
* **Half Rate Shading:** **OFF** (This is a battery saving trick meant for handhelds; on a desktop PC, it will just make your shadows look like pixelated garbage. Seriously, keep it off!)
* **Scaling Mode:** `FIT`. This is honestly just personal preference, but I prefer Fit so it uses the exact resolution I want without stretching the image weirdly. But like I said, it's up to you ;)

---

## 🚀 My Personal Proton Experience & Launch Commands

### Why you NEED GE-Proton!
You can probably just launch the game without touching the compatibility tab, but you will get awful perfomance. In my case, playing on an ultrawide monitor (which already takes a hit on performance :( , my experience was around 80 to 90 FPS with a bunch of bad lows. 

That's when I went into the tab and activated **Proton Experimental**, which surprisingly gave me between 100 to 120 FPS, and around 80 to 90 inside my base (keep in mind I had a lot of things built in the same base and it was right in the middle of the forest). 

But I still felt my rig could do more. So I activated **GE-Proton** specifically version **GE-Proton10-28** (at the time of publishing this guide, but I reccomend updating to the latest one :D). I loaded into the game and BOOM: 130 to 150 FPS, and 90 to 100 in my base! 

At first, without Experimental or GE, my GPU was sitting at around 60% usage and my CPU at 55%, which is weird. Once you activate Experimental, you will see a shift where the GPU jumps to 100% (don't worry, this is fine! :D) and the processor drops to 40%. With GE-Proton, the change was in the CPU which sat at around 30 to 35% usage. (I do recommend checking the temperature of both, that *can* be a concern, but the capacity is good like this :D. Also keep in mind that I have a mini CPU/GPU bottleneck on my end, but those are just details :D).

### The Magic Launch Command
Go to the game's Properties in Steam and drop this into the Launch Options:

```bash
RADV_PERFTEST=sam %command%
```
*(Note: If you saw `OBS_VKCAPTURE=1` in the image, don't worry about it that's just something I use for recording and streaming. For the game itself, you only need the SAM command).*

I got this info from a Reddit thread. I don't know if it's a placevo effect, but I definitely noticed a change in the amount of stutters and a solid improvement in my 1% low FPS! If you want to dive deeper, I recommend reading this thread: [Quick heads up about something I discovered](https://www.reddit.com/r/linux_gaming/comments/v58ts5/quick_heads_up_about_something_i_discovered/). There is more out there, but this gave me the foundation for it. You might as well type it in, you lose nothing :D 

**Important:** You MUST have *Resizable BAR* enabled in your computer's BIOS first, otherwise it possibly won't do anything :D Also, this command is a Linux driver trick! ;)

---

## 📝 Author's Note :D
Setting this up can seem daunting at first, but getting the configuration right just once lets you forget about the technical stuff and focus entirely on the fun later.

I hope this fast setup guide helps you focus on building your base and fighting mutants rather than tweaking settings in menus for hours.

---
## 📖 Read the Full Guide
If you prefer to read this guide with rich formatting, see the step-by-step screenshots, or want to drop a comment to the community, check out the official Steam version right here:

👉 **[Read and Favorite the Official Steam Guide Here](https://steamcommunity.com/sharedfiles/filedetails/?id=3748903209)**

---

> ***Disclaimer:*** This technical guide was written and formatted by ThatGVguy to help the Linux and gaming community optimize their game setups. 
>
> ***Technical Note:*** The environment variables and Proton configurations provided are standard, safe system-level tweaks for Bazzite. Applying custom launch options is always done at your own discretion.
>
> ***Editing Process:*** Digital creation and language assistance tools were utilized during the final proofreading of this guide to ensure clear, concise, and accurate technical instructions.

*Happy surviving and watch out for the locals!! :D*
