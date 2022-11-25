# Description

This applet is intended for owners of laptops with Nvidia hybrid graphics (Intel + Nvidia, AMD + Nvidia) running Linux with the KDE Plasma desktop environment. It is designed to make it easy to run applications on a discrete graphics card using Nvidia PRIME technology without having to relogin the session

# Why did I create it?

Relatively recently, Nvidia introduced PRIME Offloading for laptops with hybrid graphics, but did not take care of the convenience of using this technology for Linux end users. To use this technology, the user had to open a terminal and run an application through it using long and hard-to-remember environment variables. I was able to solve this by simplifying the use of this technology by reducing everything to two mouse clicks

# Notes

This applet is only for KDE Plasma users and only for laptops with Nvidia hybrid graphics

If you get a permissions error when trying to run something using the applet, check the file permissions for execution: right-click on the file, Properties -> Permisions - there should be a tick on "Is executable". If for some reason it is not checked, check it and click "OK"

![Screenshot_20221107_183831](https://user-images.githubusercontent.com/81445527/200367029-dcdc8d97-e515-431a-b563-33ebf39f1ce8.png)
![Screenshot_20221107_183906](https://user-images.githubusercontent.com/81445527/200367041-202a540e-a800-425a-9117-7cb0f068f2b1.png)

# How does he work?

Basically, it just inserts environment variables provided by Nvidia before executing the program. It works with shell-scripts, Linux executables, and .desktop files

# Requirements

1. Laptop with Nvidia hybrid graphics
2. Nvidia proprietary driver (version 430 and above)
2. KDE Plasma (any version)
3. Package kde-cli-tools (because the service calls kioclient)

# Installation

Copy the contents of the nvidia-prime-apprunner-kde directory to ~/.local/share/ (In other words: /home/your_name/.local/share/). If there is a request to replace files - agree

# Removal

Delete the file "NvidiaPrimeAppRunner.desktop" along the path ~/.local/share/kio/servicemenus/ and ~/.local/share/plasma/kickeractions/

# How to use

Just right click on the executable and click "Start on Nvidia". If you installed the applet correctly, it should appear in the context menu when you click on the file

Work tested on Asus X555LJ laptop with Intel HD Graphisc 5500 + Nvidia GeForce 920M

![screenshot_1](https://user-images.githubusercontent.com/81445527/204018545-69e6a936-807e-4613-a047-544b5360e43a.png)
![screenshot_2](https://user-images.githubusercontent.com/81445527/204018568-d5907408-fc0c-41e2-8861-41cae5360f67.png)
![screenshot_3](https://user-images.githubusercontent.com/81445527/204018584-774bdd8a-76a5-4aa0-97b8-7468760d3307.png)

Happy using! =)
