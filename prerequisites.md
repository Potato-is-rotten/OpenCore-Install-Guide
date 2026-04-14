# OpenCore入门

在着手构建基于 OpenCore 的系统之前，我们需要先了解一些事项。

## 前提条件

1. <span style="color:red">_**[关键]**_</span> 时间和耐心。
   * 如果你有重要工作或者截止日期，请不要开始这项工作，黑苹果不应该作为您日常生活的主要工作。
2. <span style="color:red">_**[关键]**_</span> **了解你的硬件**
   * 您的 CPU 型号及代号
   * 您的 GPU
   * 您的存储设备 (硬盘/固态硬盘, NVMe/AHCI/RAID/IDE 配置)
   * Your laptop/desktop model if from an OEM
   * Your **Ethernet chipset**
   * Your WLAN/Bluetooth chipset
3. <span style="color:red">_**[关键]**_</span> **A BASIC KNOWLEDGE OF COMMAND LINES AND HOW TO USE A TERMINAL/COMMAND PROMPT**
   * This is not just [关键], this is the basis of this whole guide. We can't help you if you don't know how to `cd` to a directory or delete a file.
4. <span style="color:red">_**[关键]**_</span> A machine that is compatible as seen in the _**Compatibility**_ section.
   * [Hardware Limitations page](macos-limits.md)
5. <span style="color:red">_**[关键]**_</span> A minimum of:
   * 16GB USB if you're going to use macOS to create the USB
   * 4GB USB if you're going to use Windows or Linux for USB creation
6. <span style="color:red">_**[关键]**_</span> An **Ethernet connection** (no WiFi dongles, Ethernet USB adapter may work depending on macOS support) and you must know your LAN card's model
   * You must either have a physical Ethernet port, or a compatible macOS Ethernet dongle/adapter. In case you have a [compatible WiFi card](https://dortania.github.io/Wireless-Buyers-Guide/), you can also use that.
     * Note the majority of WiFi cards are not supported by macOS
   * For people who can't use ethernet but have an Android phone, you can connect your Android phone to WiFi and then tether it using USB with [HoRNDIS](https://joshuawise.com/horndis#available_versions).
7. <span style="color:red">_**[关键]**_</span> **Proper OS Installation:**
   * Be it:
     * macOS (a fairly recent one would be better)
     * Windows (Windows 10, 1703 or newer)
     * Linux (Clean and properly functioning, with Python 2.7 or later)
   * For Windows or Linux users, **15GB** of free space on the drive you're working on. On Windows, your OS disk (C:) must have at least **15GB** of free space.
   * For macOS users, **30GB** of free space on the system's drive.
   * Most tools used in this guide will also require [Python installed](https://www.python.org/downloads/)
8. <span style="color:red">_**[关键]**_</span> **Latest BIOS installed**
   * In most cases, updating your BIOS will provide the best support for macOS
   * The exception to this are MSI 500-series AMD motherboards, read more at [Motherboard Support](macos-limits.md#motherboard-support)
