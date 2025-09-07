---
layout: default
---

## Download Windows Server 2022 ISO

Windows server 2022 ISO can be downloaded [here](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2022). When downloading, you can insert any information you want in the form but it does require a valid email.

Choose the 64 bit ISO edition.

![Branching](https://gt-legend.github.io/assets/img/win_serv-2022/iso_download.PNG)

## Create the Windows Server 2022 Virtual Machine

#### 1. Open VMware Workstation 17 Pro

* Launch VMware Workstation after installation.

#### 2. Create a New Virtual Machine

* Click on "Create a New Virtual Machine."

* Choose between the Typical (recommended) or Custom configuration. For beginners, Typical is usually the easiest option.

#### 3. Select the Installation Media

* Choose "Installer disc image file (iso)" and browse to the location where you saved your Windows Server 2022 ISO file.

![Branching](https://gt-legend.github.io/assets/img/win_serv-2022/product_key.PNG)

#### 4. Select a Guest Operating System

* Choose Microsoft Windows as the guest operating system and select Windows 10 from the version dropdown. Click Next.

#### 5. Name the Virtual Machine

* Give your VM a name and choose the location for storing the VM files. Ensure that you have enough local disk space available.

#### 6. Specify Disk Capacity

* Enter the maximum disk capacity. It is recommended to allocate at least 64 GB to accommodate the operating system and applications. Choose whether to store the virtual disk as a single file or split it into multiple files. Single files generally perform better.

#### 7. Customize Hardware (Optional)

* Click on Customize Hardware to allocate resources such as RAM, CPU cores, and network preferences.

* Memory: For Windows 10, at least 4 GB is required. However, if your host allows, allocate 8 GB or more for better performance.

* Processors: Allocate at least 2 cores for a smoother experience.

* Network Adapter: Set it to NAT or Bridged based on your network configuration.

* Ensure that the "Accelerate 3D graphics" option is enabled for graphic-intensive applications.

* If TPM is required, you can add a Trusted Platform Module through the hardware settings.

#### 8. Finish Configuration

* Once configured, click Close, then Finish to create your virtual machine.


[Back](/projects/home_lab.html)