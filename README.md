# GPL v3 in a nutshell [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
You may copy, distribute and modify the software as long as you track changes/dates in source files. Any modifications to or software including (via compiler) GPL-licensed code must also be made available under the GPL along with build & install instructions.

# Universal PC Optimization
Universal PC Optimization is your go-to guide for all things related to enhancing your PC's performance! This release is designed to help users of all skill levels unlock the full potential of their computers. Inside, you'll find a wealth of valuable information on PC tweaking and fine-tuning, helping you optimize every aspect of your system's performance. Whether you're dealing with software errors, hardware failures, or just looking to squeeze out every last bit of speed from your setup, Universal PC Optimization has you covered. Dive in now to learn the best practices for keeping your PC running smoothly and efficiently! Feel free to contribute!

## Disclaimer
> [!CAUTION]
> Operate at your own risk!

The information provided in Universal PC Optimization is intended for educational and informational purposes only. While every effort has been made to ensure the accuracy and reliability of the content, it is important to understand that all advice, tips, and suggestions are to be used at your own risk.

Modifying system settings, tweaking hardware, and making changes to your PC can have unintended consequences. Always double-check any modifications or changes against the manufacturer’s guidelines and documentation. The authors and contributors of this guide are not liable for any damages, loss of data, or hardware failures that may result from following the information provided. Proceed with caution and always make sure to back up your data before making any changes to your system.


## Why I decided to create this
<details>
  <summary>Little story of troubleshooting issues with my PC</summary>
<br>
Thank you for taking the time to read my story.
  <br><br>
I'll start by describing my PC's behavior. For several days, I had been experiencing severe frame drops and stuttering while gaming. That's why I decided to "debug" my hardware and software to discover the cause of these issues and, ultimately, fix them. I'm glad to say that, by the end of my journey, during which I learned about many topics I was previously unaware of, I managed to fully resolve all my problems. Now, I'm enjoying stable frame rates while gaming, along with consistent CPU usage, temperature, energy consumption, and performance.

The guide below is a kind of story about all the steps I took to debug and identify the root cause of my issue.

  </details>


I'll divide the guide into multiple chapters to improve readability and split it into 2 Macro topics: Software and Hardware
- [Software](#software)
  - [Update Windows](#update-windows)
  - [Verify Windows](#verify-windows)
  - [Optimize Windows](#optimize-windows)
  - [Windows Tweaks](#windows-tweaks)
  - [Network Tuning](#network-tuning)
  - [Game Optimization](#game-optimization)
  - [Steps](#steps)
- [Hardware](#hardware)
  - [Basic Usage](#basic-usage)
  - [Advanced Usage](#advanced-usage)

# Software
## Update Windows
It might sound obvious, but keeping Windows, drivers, and software updated is the first step to maintaining a fully functioning machine.

Always refer to your component manufacturers and ensure you download the correct drivers and updates.

I don't recommend using software that automatically updates your drivers; Windows Update is more than sufficient.

## Verify Windows
To ensure the integrity of your Windows installation, I highly recommend running the following commands in Command Prompt (preferably as an administrator):

```chkdsk``` - Verifies the integrity of disk sectors.

```sfc /scannow``` - Scans and repairs system files to verify system integrity.

```Dism /Online /Cleanup-Image /CheckHealth``` - Checks for component store corruption.

```Dism /Online /Cleanup-Image /ScanHealth``` - Scans the component store for corruption.

```Dism /Online /Cleanup-Image /RestoreHealth``` - Repairs the component store to restore system health.

If you are using an x64 Windows version, you can use my [PCNukerPro](https://github.com/NazgulCoder/PCNukerPro)

## Optimize Windows
It might sound odd, but many people believe that Windows is a perfect environment where everything should work flawlessly. Hard pill to swallow: it's not!

Windows comes with a lot of unnecessary software installed by default, and many manufacturers add their own bloatware. Fortunately, there are many tools available to de-bloat your system and improve performance.

One of my favorite tools for this purpose is [Optimizer](https://github.com/hellzerg/optimizer)

I recommend enabling the <ins>**Optimize Performance**</ins> option and turning on <ins>**Gaming Mode**</ins>. If your games or apps do not require it, I highly recommend turning off <ins>**Xbox Live**</ins> and the <ins>**Game Bar**</ins>.

You can also disable app telemetry to improve your privacy and slightly enhance performance.

Other honorable mentions for fine-tuning your PC, cleaning it of junk, and improving overall performance and stability are:
- [dMaintenance Home Edition](https://www.d7xtech.com/dmaintenance-home-edition/)
- [Tweaky](https://www.d7xtech.com/tweaky/) 
- [CCleaner](https://www.ccleaner.com/ccleaner/download) - Mainly used for cleaning, fixing the registry, uninstalling apps, and removing unwanted apps from startup - **BEWARE OF INTRUSIVE ADS**
- [AdwCleaner](https://www.malwarebytes.com/adwcleaner) - Remove Bloatwares

## Windows Tweaks
I recommend to disable [GameBarPresenceWriter](https://github.com/NazgulCoder/Universal-PC-Optimization/raw/refs/heads/main/uploads/Disable%20GameBarPresenceWriter.zip) and [MPO](https://github.com/NazgulCoder/Universal-PC-Optimization/raw/refs/heads/main/uploads/MPO.zip) to improve gaming performance by minimizing background interference and ensuring GPU and CPU resources are fully dedicated to the game. These optimizations are particularly beneficial for gamers experiencing stuttering, input lag, or screen tearing, especially in competitive settings where every millisecond counts. Disabling these features helps prioritize raw performance over non-essential functionalities, leading to a smoother and more consistent gaming experience.

I recommend also following these steps to tune your Windows for optimal performance:

- **Daily Drive Optimization**  
   Go to **Settings > System > Storage > Advanced storage settings > Drive optimization**. Click **Optimize** for each drive and enable **Scheduled optimization**.

- **Display Refresh Rate**  
   Go to **Settings > System > Display > Advanced display settings**. Under **Refresh rate**, select the highest available refresh rate for your monitor.

- **Advanced Windows Graphics Settings**  
   Go to **Settings > System > Display > Graphics settings**. Enable **Hardware-accelerated GPU scheduling** if available.

- **Windows Storage Sense**  
   Go to **Settings > System > Storage** and enable **Storage Sense** to automatically free up space.

- **Nvidia App (or GPU Software)**  
   Open **Nvidia Control Panel** or the relevant software (e.g., AMD or Intel GPU control panel). Configure **3D settings** for optimal performance. You may want to enable G-Sync as well.

- **Global Low Latency Mode**  
    In **Nvidia Control Panel**, go to **Manage 3D settings > Low Latency Mode** and set it to **On** or **Ultra** for minimal input lag.

- **ShadowPlay Settings**  
    Open **GeForce Experience > Settings > In-Game Overlay**. Configure **ShadowPlay** options like instant replay or recording settings based on your preference. If you want maximum performance then disable it.

- **Disable Unneeded Audio Devices**  
    Right-click the **Speaker icon** > **Sounds** > **Playback/Recording tabs**. Disable any unused audio devices to reduce system overhead.

> [!CAUTION]
> **High Performance Mode** <br>
> This setting may cause high temperatures. <br>
> Go to **Settings > System > Power & sleep > Additional power settings**. Select **High performance** or **Ultimate performance** (if available).

## Network Tuning

### General Online Gaming Recommendations

I recommend the following steps to optimize your online gaming experience:

- **Use Brand-Name Wired Ethernet Cards**: Whenever possible, use brand-name wired Ethernet cards instead of Wi-Fi, especially with USB client adapters, to ensure a stable connection.
  
- **TCP/IP Tweaks**: When tweaking TCP/IP (following our general tweaking articles), enable **CTCP**, enable **DCA**, and consider disabling most "TCP Offloading" settings, except for "Checksum Offload" in both the OS and Network Adapter Properties.

- **Network Adapter Settings**: Disable **Flow Control** and **Interrupt Moderation** in your Network adapter properties. If you're not using IPv6, disable **TCP/IPv6** in the Network adapter properties as well.

- **Background Processes**: Reduce the number of background processes running on your system, enable **QoS** at your router, and give priority to your gaming traffic.

- **Test Latency**: Test your latency to game servers using the `tracert` command in Command Prompt (or PowerShell) to diagnose any connectivity issues.

- **Disable Search Indexing**: Disable search indexing on your SSD/hard drive by right-clicking on the drive in Explorer, selecting **Properties**, and unticking **Allow files on this drive to have contents indexed...**. Wait a few minutes and ignore errors for system-protected files.

- **Close Unnecessary Programs**: Close unnecessary programs running on your network via Task Manager (Ctrl + Shift + Escape). P2P applications like uTorrent and Skype can consume bandwidth by opening many sockets for passive listening. Additionally, programs that check for software updates (e.g., Google updates, Adobe updates) can cause ping spikes.

### Intel Recommended Network Adapter Settings

For optimal performance, consider the following settings based on your needs:

### Optimized for Quick Response and Low Latency (Gaming):
- Minimize or disable **Interrupt Moderation Rate**.
- Disable **Offload TCP Segmentation**.
- Increase **Transmit Descriptors**.
- Increase **Receive Descriptors**.
- Increase **RSS Queues**.

### Optimized for Throughput:
- Enable **Jumbo Frames**.
- Increase **Transmit Descriptors**.
- Increase **Receive Descriptors**.

### For Low CPU Utilization:
- Maximize **Interrupt Moderation Rate**.
- Keep **Receive Descriptors** at default.
- Avoid setting large **Receive Descriptors**.
- Decrease **RSS Queues**.
- Decrease the maximum number of **RSS CPUs** in Hyper-V environments.

A big vouch to SpeedGuide for providing these settings! I also recommend checking out their full guide [here](https://www.speedguide.net/articles/gaming-tweaks-5812) or [here for offline read](https://github.com/NazgulCoder/Universal-PC-Optimization/blob/main/uploads/SG%20__%20Gaming%20Tweaks.mhtml) and using **TCP Optimizer** with their profiles for even better performance.

## Game Optimization

To get the best performance in games, I personally recommend the following steps:

### Use RivaTuner to Cap FPS
- **Why cap FPS?** Capping your FPS can reduce input lag, prevent screen tearing, and lower GPU/CPU usage, keeping temperatures down.
- **How to cap FPS:**
  1. Install **MSI Afterburner** (RivaTuner Statistics Server comes bundled with it).
  2. Open **RivaTuner Statistics Server (RTSS)**.
  3. Add your game’s executable if it isn’t listed.
  4. Set the **Framerate limit** to a value just below your monitor’s refresh rate (e.g., 141 FPS for a 144Hz monitor).

This helps maintain smooth gameplay without unnecessary performance spikes.

### Optimize In-Game Settings
- **Resolution and Refresh Rate**: Always match the resolution and refresh rate to your monitor’s native specs.
- **Graphics Settings**:
  - **Textures**: Use High/Ultra only if your GPU has enough VRAM (6GB+ recommended). Otherwise, set to Medium.
  - **Shadows**: Shadows are GPU-intensive—lower them if you’re struggling with FPS.
  - **Anti-Aliasing (AA)**: If performance is a concern, use **TAA** or **FXAA**. Avoid higher AA settings like MSAA unless you have extra headroom.
  - **V-Sync**: Turn off V-Sync if you're using a capped FPS or G-Sync/FreeSync to reduce input lag.
  - **Field of View (FOV)**: A wider FOV may reduce FPS. Stick to a reasonable FOV that balances visibility and performance.

### Disable Unnecessary Background Processes
- **Game Mode**: Turn on **Windows Game Mode** to optimize resource allocation.
- **Windows Notifications**: Disable notifications while gaming to avoid interruptions.
- **Background Programs**: Use **Task Manager (Ctrl + Shift + Esc)** to close unneeded processes like Discord overlays, browsers, or any software updates running in the background.

### Use a Game-Specific Config File (Optional)
- Many games allow advanced tweaking through **config files** (e.g., `game.cfg` or `settings.ini`).
  - Look for performance-related values like **MaxFPS**, **Draw Distance**, or **Shadow Quality**.
  - Backup the original config before making changes, and tweak based on your system’s specs.

A smooth gaming experience often comes down to balancing graphics settings with performance. Take the time to find what works best for your setup, and don't forget to monitor **temps** with MSI Afterburner or HWMonitor.


WORK IN PROGRESS
