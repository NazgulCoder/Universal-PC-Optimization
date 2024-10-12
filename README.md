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

I recommend also to enable daily drive optimization. To do so, go to **Settings > System > Storage > Advanced storage settings > Drive optimization**, click **Optimize** for your drives, and make sure **Scheduled optimization** is turned on for automatic maintenance.




WORK IN PROGRESS
