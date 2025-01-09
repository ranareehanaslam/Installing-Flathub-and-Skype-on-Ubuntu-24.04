# 🛠️ Installing Flathub and Skype on Ubuntu 24.04

Welcome to the guide for setting up Flathub on Ubuntu 24.04 and installing Skype using Flatpak. Follow these steps to enjoy a seamless installation process.

## 📋 Prerequisites

- A system running Ubuntu 24.04 or later.
- Administrative (sudo) access to your system.

## Step 1: Install Flatpak

Flatpak is included in the software sources of Ubuntu 18.10 and later. To install it, open a terminal and run:

```bash
sudo apt install flatpak
```

For older versions of Ubuntu (up to 18.04 LTS), you need to add the official Flatpak PPA:

```bash
sudo add-apt-repository ppa:flatpak/stable
sudo apt update
sudo apt install flatpak
```

## Step 2: Install the GNOME Software Flatpak Plugin

The GNOME Software plugin allows you to install Flatpak apps without using the command line. Install it by running:

```bash
sudo apt install gnome-software-plugin-flatpak
```

**Note:** On Ubuntu versions 20.04 to 23.04, GNOME Software is distributed as a Snap package and does not support Flatpak apps. Installing this plugin will install a deb version of GNOME Software, resulting in two "Software" apps being installed. For Ubuntu 23.10 and newer, a single new "Software" app will be installed.

## Step 3: Add the Flathub Repository

Flathub is the go-to repository for Flatpak apps. To enable it, run:

```bash
flatpak remote-add --if-not-exists flathub https://dl.flathub.org/repo/flathub.flatpakrepo
```

## Step 4: Restart Your System

Restart your system to finalize the setup:

```bash
sudo reboot
```

## Step 5: Install Skype

Once Flatpak and Flathub are set up, you can easily install Skype by running:

```bash
flatpak install flathub com.skype.Client
```

## Step 6: Launch Skype

To launch Skype after installation, run the following command in the terminal or search for "Skype" in your application menu:

```bash
flatpak run com.skype.Client
```

## 📚 Additional Resources

- [Flatpak Documentation](https://flatpak.org/)
- [Flathub Repository](https://flathub.org/)
- [Skype on Flathub](https://flathub.org/apps/details/com.skype.Client)

Enjoy using Flathub and Skype on Ubuntu 24.04! 🎉
```

This `README.md` provides clear instructions with step-by-step commands and includes icons to make the guide more engaging. The additional resources section offers direct links for further information.

For more information on Flatpak and Flathub, visit the official Flathub website:  
