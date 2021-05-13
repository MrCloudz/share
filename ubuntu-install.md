# Ubuntu Server Installation

You'll need:

- A USB with 2gb of free storage space.
- Take a backup of your existing OS install, if you have one.

Step 1

- Open https://ubuntu.com/download/server
- Select "manual server installation".

You now have an ``Iso file`` for Ubuntu server!

Step 2:

- Download Rufus https://rufus.ie
- Select the Rufus installer from your downloads and follow the steps.

Rufus will flash this ISO file to your USB drive.

Step 3

- Plug in your USB drive and open Rufus from your downloads.
- Click "show advanced drive properties"
- Click "show hard drives"
- Under the "device" option, select the drive you want to flash Ubuntu server on.
- Select "START"!

[WARNING]: This will destory all content on your USB device. Insure you have a backup.

Step 4

Enter your motherboard BIOS and boot from this USB, you'll need to refer to the user-manual of your motherboard.

Step 5

Awesome! So now you're booting into Ubuntu. Ubuntu server will do some checks of your install and you're all good!

You'll be asked some setup questions, this will change depending on your install version.

# Cool things you can install on Ubuntu server!

Firstly, you'll want to run ``sudo apt update`` to update your install, then you'll want to run ``sudo apt-get update`` to update your repositories.

# Installing .NET.

``"The .NET Framework is a software framework developed by Microsoft that runs primarily on Microsoft Windows. It includes a large class library called Framework Class Library and provides language interoperability across several programming languages." - Wikipedia``

https://dotnet.microsoft.com

The official documentation for installing .NET on Linux is here https://docs.microsoft.com/en-nz/dotnet/core/install/linux

However, here's the basics.

[Warning]: .NET only works on versions 20.10, 20.04, 18.04, 16.04.

Here are the steps for 20.10.

Run these commands in your terminal.

```
wget https://packages.microsoft.com/config/ubuntu/20.10/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
sudo dpkg -i packages-microsoft-prod.deb

sudo apt-get update; \
  sudo apt-get install -y apt-transport-https && \
  sudo apt-get update && \
  sudo apt-get install -y dotnet-sdk-5.0
```

You'll all set!

# Node.js

Run these commands:

``sudo apt-get install nodejs``

Done!

# MySQL Commmunity

Run these ommands;

``sudo apt install mysql-server``

``sudo mysql_secure_installation``

You can follow the installation prompts!

Done!

# Commands in Linux.

As you've probably noticed. Installing things on Linux is super easy! It isn't very complex.

# Congradulations, you've installed Ubuntu server!
