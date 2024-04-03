---
author: Brian
title: VirtualBox Install On Debian 12
slug: /virtualbox-install-on-debian-12
date: 2024-04-02T19:14:05-04:00
draft: false
# layout: 
# description: 
tags: Linux
# icon: 
thumbnail: 
    url: img/debian_virtualbox.webp
    author: DALL-E
    authorURL: https://openai.com/dall-e-3
    # origin: 
    # originURL: 
---
## What is VirtualBox
VirtualBox is a free and open source Type-2 hypervisor owned and maintained by Oracle. A Type-2 hypervisor means it runs as an application on an operating system. This means you can run VirtualBox on your Linux, Mac, or Windows computer. In this post, we will install VirtualBox on Debian 12. If you're following along and you are not running Debian 12, don't worry! These instructions should work on all Debian-based linux distributions.

## Installing VirtualBox
#### Step 1

Check and install any updates
{{< command >}}
sudo apt update && sudo apt upgrade -y
{{< /command >}}

#### Step 2
Install required packages
{{< command >}}
sudo apt install gcc make linux-headers-$(uname -r) dkms -y
{{< /command >}}

#### Step 3
Add the Oracle VirtualBox public key
{{< command >}}
curl https://www.virtualbox.org/download/oracle_vbox_2016.asc | sudo gpg --dearmor --yes --output /etc/apt/trusted.gpg.d/vbox.gpg
{{< /command >}}

#### Step 4
Add the Oracle VirtualBox repository
{{< command >}}
echo "deb [arch=amd64] http://download.virtualbox.org/virtualbox/debian bookworm contrib" | sudo tee /etc/apt/sources.list.d/virtualbox.list
{{< /command >}}

#### Step 5
Update the repositories and install the latest version of VirtualBox
{{< command >}}
sudo apt update && sudo apt install virtualbox-7.0 -y
{{< /command >}}

#### Step 7
Add your current username to the vboxusers users group
{{< command >}}
sudo usermod -aG vboxusers $USER
{{< /command >}}

## Wrapping Up
We are now ready to start building virtual machines using VirtualBox. I hope you found this short install guide helpful.

Stay curious,

-Brian

Helpful Links
https://www.virtualbox.org/manual/UserManual.html#install-linux-host