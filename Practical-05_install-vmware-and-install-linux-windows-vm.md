# Practical 5

Source PDF: Practical 5.pdf

--- Page 1 ---

Practical 5
AIM: Install VMware and Install Linux/Windows VM

To install a virtualization software such as VMware and create a virtual machine to run a Linux or Windows
operating system.



What Is VMware?

VMware is a virtualization technology company that provides software and solutions for creating, running, and
managing virtual machines (VMs) and virtualized infrastructure.

VMware allows one physical computer/server to run multiple virtual machines, each with its own operating system
and applications.

For example, one physical server can run:

    •   Windows Server VM

    •   Ubuntu Linux VM

    •   Red Hat Linux VM

All three can run on the same physical hardware.

VMware Workstation
Desktop software used to create and run VMs on a host computer.



Steps Of Implementation

Requirements
    •   Computer/Laptop

    •   VirtualBox or VMware Workstation

    •   Linux/Windows ISO file

    •   Minimum 4 GB RAM recommended

    •   At least 30–50 GB free disk space

Part A: Install VirtualBox/VMware
    1. Download VirtualBox or VMware Workstation from its official website.

        https://www.techpowerup.com/download/vmware-workstation-pro/

    2. Run the downloaded installer.

    3. Accept the license agreement.

    4. Select the installation location.

    5. Click Install.

    6. Wait until the installation is completed.

--- Page 2 ---

7. Click Finish

    8. Open VMware Workstation.



Part B: Download the ISO File
        ISO (International Organization for Standardization) is an organization that develops international
        standards.

        In computing, an ISO file is a disk image file that contains an exact copy of the contents of a CD, DVD, or
        installation media.



        Steps

    1. Open the official website of the operating system.

        https://www.microsoft.com/en-gb/software-download/windows11arm64

    2. Download the required ISO file.

            o    For Linux → Ubuntu/RHEL ISO

            o    For Windows → Windows ISO

    3. Save the ISO file on your computer.

    4. Make sure the .iso file is completely downloaded.

Note: The ISO file is not installed separately. It is used as the installation media for the virtual machine.



Part C: Create a New Virtual Machine
    1. Open VMware Workstation.

    2. Click Create a New Virtual Machine.

    3. Select Typical (Recommended).

    4. Click Next.

    5. Select Installer disc image file (ISO).

    6. Click Browse.

    7. Select the downloaded ISO file.

    8. Click Next.

    9. Select the appropriate Operating System type and version.

    10. Enter a Virtual Machine Name, e.g. Ubuntu VM or Windows 11 VM.

    11. Select the location where you want to store the VM.

    12. Set the Virtual Hard Disk size, e.g. 30 GB.

    13. Allocate RAM, e.g. 2–4 GB.

    14. Configure CPU if required.

--- Page 3 ---

15. Review the VM configuration.

    16. Click Finish.

Part D: Start the Virtual Machine
    1. Select the newly created VM.

    2. Click Power On.

    3. VMware starts the virtual machine.

    4. The VM boots from the selected ISO file.

    5. The operating system installation screen appears.



Part E: Install the Operating System
    1. Select the required Language.

    2. Select Keyboard Layout.

    3. Select Region/Time Zone if required.

    4. Click Install.

    5. Follow the OS installation wizard.

    6. Select the virtual hard disk as the installation location.

    7. Create a username and password when prompted.

    8. Wait while the operating system files are copied and installed.

    9. The VM may restart automatically.



Part F: Complete the Installation
    1. After restarting, the VM boots into the newly installed OS.

    2. Complete the initial setup.

    3. Log in using the username and password.

    4. Verify that the OS is working properly.



Final Result

VMware Workstation → New VM → Attach ISO → Allocate RAM/CPU/Disk → Power On → OS Installation → OS
Running
