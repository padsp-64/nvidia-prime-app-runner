# Description

This applet is intended for owners of laptops with Nvidia hybrid graphics (Intel + Nvidia, AMD + Nvidia) running Linux with the KDE Plasma desktop environment. It is designed to make it easy to run applications on a discrete graphics card using Nvidia PRIME technology without having to relogin the session

# Why did I create it?

Relatively recently, Nvidia introduced PRIME Offloading for laptops with hybrid graphics, but did not take care of the convenience of using this technology for Linux end users. To use this technology, the user had to open a terminal and run an application through it using long and hard-to-remember environment variables. I was able to solve this by simplifying the use of this technology by reducing everything to two mouse clicks

# Note

This applet is only for KDE Plasma users and only for laptops with Nvidia hybrid graphics

# How does he work?

Basically, it just inserts environment variables provided by Nvidia before executing the program. It works with shell-scripts, Linux executables, and .desktop files

# Requirements

1. Laptop with Nvidia hybrid graphics
2. KDE Plasma (any version)
3. Package kde-cli-tools (because the service calls kioclient)

# Installation

Copy the contents of the nvidia-prime-apprunner-kde directory to ~/.local/share/ (In other words: /home/your_name/.local/share/). If there is a request to replace files - agree

# Removal

Delete the file "NvidiaPrimeAppRunner.desktop" along the path ~/.local/share/kio/servicemenus/ and ~/.local/share/plasma/kickeractions/

# How to use

Just right click on the executable and click "Run on Nvidia". If you installed the applet correctly, it should appear in the context menu when you click on the file
