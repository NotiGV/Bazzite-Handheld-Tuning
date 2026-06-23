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

<img width="400" height="400" alt="Bazzite_Logo-ThatGVguy" src="https://github.com/user-attachments/assets/d163786e-c5d7-458c-b026-e3c8afaa79b3" />

* **CPU:** AMD Ryzen 5 5600

<img width="400" height="400" alt="AMD Ryzen 5 5600" src="https://github.com/user-attachments/assets/3d3bb854-19e6-4ed9-9e53-9770980fbaae" />

* **GPU:** ASRock Challenger Radeon RX 7800 XT OC (16GB VRAM)

<img width="600" height="350" alt="DUALFANDESIGN-Radeon RX 7800 XT Challenger 16GB OC_mobile" src="https://github.com/user-attachments/assets/8e2d7b3f-c18d-46c6-8024-21abb262e3a2" />

* **RAM:** 16 GB (2x8) T-Force Delta R @ 3200MHz

<img width="400" height="400" alt="16 GB (2x8) T-Force Delta R @ 3200MHz" src="https://github.com/user-attachments/assets/4bf406a5-492b-44d6-bd5f-1f49c96788bb" />

* **Monitor:** Xiaomi G34WQi (Ultrawide 21:9, 1440p, 180Hz)

<img width="600" height="600" alt="_Xiaomi G34WQi" src="https://github.com/user-attachments/assets/c39f4439-155b-498e-b825-44a478ea7dea" />

---

## 🌲 In-Game Settings (The Sweet Spot)
*This setup maintains maximum visual quality while eliminating those annoying blurry cinematic filters. It also reduces a few "Ultra" options that bottleneck your CPU without giving you any real visual benefit.*

<img width="2264" height="1160" alt="The Forest-Options Menu-ThatGVguy-bazzite" src="https://github.com/user-attachments/assets/9521425f-3a22-4920-8d23-df1059e0db1f" />

### Left Column Settings

<img width="1094" height="844" alt="The Forest-Options Menu 1-ThatGVguy-bazzite" src="https://github.com/user-attachments/assets/dd351f0b-d3ce-4f85-9cfe-789c0bf562ef" />

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

<img width="1094" height="844" alt="The Forest-Options Menu 2-ThatGVguy-bazzite" src="https://github.com/user-attachments/assets/8a58f56c-ba7e-4b16-9dc0-ca75c2c639be" />

**(Quick note here: You can honestly set most of these to Ultra, but to be honest there isn't much of a difference in my opinion, so save those frames for smoother gameplay!)**

* **Ocean Quality:** `LOW`. This one is dynamic! If you go to the ocean a lot or live there and want to see as best as possible underwater, **Flat** is without a doubt the best option (the water gets way more transparent). 

<img width="3440" height="1440" alt="The Forest-ThatGVguy-bazzite-Flat Ocean Quality" src="https://github.com/user-attachments/assets/5e880388-e650-44ae-8ca1-741cf4b1d807" />

But if you want a realistic experience, **Low** 

<img width="3440" height="1440" alt="The Forest-ThatGVguy-bazzite-low ocean quality" src="https://github.com/user-attachments/assets/035f1fd4-22de-425c-80a4-69d3b54bc93f" />

And **High** are fine. 

<img width="3440" height="1440" alt="The Forest-ThatGVguy-bazzite-High Ocean Quality" src="https://github.com/user-attachments/assets/3c78e184-cbd8-4e83-b405-fe80817d934a" />

I personally keep it on *Low* because I almost never visit the ocean anyway :D
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

<img width="3440" height="1440" alt="The Forest-ThatGVguy-bazzite-Processing Shaders" src="https://github.com/user-attachments/assets/6280566b-cb70-401a-9597-9ae621a2eb1e" />

**💡 Quick Tip:** When you launch the game, you might see a small Steam window popping up saying it's processing Vulkan shaders. Just let it finish! It takes 10 seconds at most, and your in game perfomance will seriously thank you later! :b 

*These are the tweaks you apply in the quick access performance menu (the one you open with the three-dot button or Home button + A on Xbox Layout/ X on Playstation / B on Switch).*

<img width="3440" height="1440" alt="The Forest-ThatGVguy-bazzite-Steam Quick Access Performance Menu" src="https://github.com/user-attachments/assets/d849d575-fdc2-4234-aeba-1c323d52e377" />

<img width="667" height="1276" alt="The Forest-ThatGVguy-bazzite-Steam Quick Access Performance Menu 2" src="https://github.com/user-attachments/assets/a9234d9b-8ac7-4366-a560-64426fde7f87" />

* **Frame Limit:** Set this about **5 to 8 FPS below your monitor's maximum**. Why? Because if you hit your absolute max refresh rate, you step outside your VRR/FreeSync window and V-Sync forces itself on, giving you annoying input lag. Capping it just below the limit keeps everything buttery smooth and responsive!
* **Enable VRR (FreeSync):** **ON** (This makes sure your monitor syncs perfectly with your FPS so you don't feel any stutters).
* **Enable HDR:** **OFF** (The game just doesn't support it natively).
* **Allow Tearing:** **OFF** (Since we have VRR active, leaving this on would just cause unnecesary visual tearing).
* **Half Rate Shading:** **OFF** (This is a battery saving trick meant for handhelds; on a desktop PC, it will just make your shadows look like pixelated garbage. Seriously, keep it off!)
* **Scaling Mode:** `FIT`. This is honestly just personal preference, but I prefer Fit so it uses the exact resolution I want without stretching the image weirdly. But like I said, it's up to you ;)

---

## 🚀 My Personal Proton Experience & Launch Commands

### Why you NEED GE-Proton!

<img width="3440" height="1440" alt="The Forest-GE proton-ThatGVguy-bazzite" src="https://github.com/user-attachments/assets/8032d135-aeb5-49cb-9af8-b7d786fd8ee6" />

You can probably just launch the game without touching the compatibility tab, but you will get awful perfomance. In my case, playing on an ultrawide monitor (which already takes a hit on performance :( , my experience was around 80 to 90 FPS with a bunch of bad lows. 

That's when I went into the tab and activated **Proton Experimental**, which surprisingly gave me between 100 to 120 FPS, and around 80 to 90 inside my base (keep in mind I had a lot of things built in the same base and it was right in the middle of the forest). 

But I still felt my rig could do more. So I activated **GE-Proton** specifically version **GE-Proton10-28** (at the time of publishing this guide, but I reccomend updating to the latest one :D). I loaded into the game and BOOM: 130 to 150 FPS, and 90 to 100 in my base! 

At first, without Experimental or GE, my GPU was sitting at around 60% usage and my CPU at 55%, which is weird. Once you activate Experimental, you will see a shift where the GPU jumps to 100% (don't worry, this is fine! :D) and the processor drops to 40%. With GE-Proton, the change was in the CPU which sat at around 30 to 35% usage. (I do recommend checking the temperature of both, that *can* be a concern, but the capacity is good like this :D. Also keep in mind that I have a mini CPU/GPU bottleneck on my end, but those are just details :D).

### The Magic Launch Command
Go to the game's Properties in Steam and drop this into the Launch Options:

<img width="3440" height="1440" alt="The Forest-ThatGVguy-bazzite-Launch options" src="https://github.com/user-attachments/assets/732fef33-5fbc-4e62-999f-0e51b1b8e3d1" />

```bash
RADV_PERFTEST=sam %command%
```
*(Note: If you saw `OBS_VKCAPTURE=1` in the image, don't worry about it that's just something I use for recording and streaming. For the game itself, you only need the SAM command).*

I got this info from a Reddit thread. I don't know if it's a placevo effect, but I definitely noticed a change in the amount of stutters and a solid improvement in my 1% low FPS! If you want to dive deeper, I recommend reading this thread: [Quick heads up about something I discovered](https://www.reddit.com/r/linux_gaming/comments/v58ts5/quick_heads_up_about_something_i_discovered/). There is more out there, but this gave me the foundation for it. You might as well type it in, you lose nothing :D 

**Important:** You MUST have *Resizable BAR* enabled in your computer's BIOS first, otherwise it possibly won't do anything :D Also, this command is a Linux driver trick! ;)

---

## ⚖️ High FPS vs Pure Fluidity (Optional)

This is a bit of a controversial topic. Everything we did above is perfect for getting the absolute highest FPS possible. But if you look closely, those frames fluctuate a lot. If you want pure, buttery smoothness, I highly recommend capping your FPS...

But wait, if we just fought for more frames, why cap them? the answer is **Frame Pacing**!

If your rig reaches around 120 to 150 FPS like mine, and your monitor is 180Hz, capping the game at **90 FPS** is the magic trick. why? Because 180 / 90 = 2. You want the result to be a clean, whole number! This means your monitor displays exactly one game frame for every two monitor refreshes perfectly, it creates a flawless, buttery sensation. You *could* do 60 FPS (180 / 60 = 3), but dropping from 150 down to 60 is very noticeable, which is why 90 is the absolute sweet spot!! :D

Here is a quick cheat sheet depending on your monitor's max Hz and what FPS your PC can comfortably hold without dropping:

* **120Hz Monitor:** Cap at 60 FPS (divided by 2).
* **180Hz Monitor:** Cap at 90 FPS (divided by 2) or 60 FPS (divided by 3).
* **240Hz Monitor:** Cap at 120 FPS (divided by 2), 80 FPS (divided by 3), or 60 FPS (divided by 4).
* **360Hz Monitor:** Cap at 180 FPS (divided by 2), 120 FPS (divided by 3), or 90 FPS (divided by 4).
* **480Hz Monitor:** Cap at 240 FPS (divided by 2), 160 FPS (divided by 3), or 120 FPS (divided by 4).

**PS: You will still notice occasional stutters.** why? Honestly, it's just the game engine. I tested it on completely Low settings and still got stutters at a locked 60 FPS. So, if you want to play *The Forest*, you just have to accept a random hiccup here and there

As a friend, I seriously recommend capping your frames using the Gamescope menu we talked about earlier. I know it sounds counterproductive after squeezing every drop of perfomance, but trust me, you will get used to the locked 90 or 120 (depending on your monitor) and it feels absolutely amazing! :D

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
