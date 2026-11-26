# Practical 7

Source PDF: Practical 7.pdf

--- Page 1 ---

Practical 7
AIM: VM Snapshot, Restore, Clone and VMware Shared Folder

To create a snapshot of a virtual machine, restore the VM using the snapshot, and create a clone
of the virtual machine.



1. VM Snapshot

A snapshot is a saved state of a Virtual Machine (VM) at a particular point in time. It records the
VM's disk state and, depending on the virtualization software/settings, its memory and
configuration state.

Purpose:

Snapshots are mainly used before making changes to a VM, such as installing software, changing
configurations, or testing something risky. If something goes wrong, the VM can be restored to the
previous snapshot.

Example:

Before installing new software → Take Snapshot → Install software → If a problem occurs →
Restore Snapshot.



2. Restore Snapshot

Restore means returning the VM to the state captured when the snapshot was taken.

When a snapshot is restored:

    •   The VM's disk state returns to the snapshot point.

    •   Changes made after the snapshot may be lost.

    •   It is useful for recovering from configuration errors or failed experiments.



3. VM Clone

A VM Clone is a copy of an existing virtual machine. The cloned VM can be used as a separate VM
without affecting the original VM.

Purpose:

    •   Quickly create another VM.

    •   Create multiple similar VMs.

    •   Use an existing configured VM as a template.

    •   Useful in testing, development and lab environments.

Example:

--- Page 2 ---

If you have a Linux VM already configured with all required software, you can clone it to create
another Linux VM instead of installing everything again.



Snapshot vs Clone

Snapshot                                         Clone

Saves the state of an existing VM                Creates a separate copy of the VM

Used mainly for backup/recovery during testing Used to create another VM

Usually depends on the original VM               Can be used as a separate VM

Helps restore the previous state                 Helps create multiple similar VMs



Practical Steps

Part A: Create a VM Snapshot

    1. Open VMware Workstation.

    2. Select the required Virtual Machine.

    3. Make sure the VM is in the required state.

    4. Go to VM → Snapshot → Take Snapshot.

    5. Enter a snapshot name, for example Before_Changes.

    6. Add a description if required.

    7. Click Take Snapshot.

    8. The snapshot will be created successfully.



Part B: Restore the Snapshot

    1. Start the VM and make some changes to it.

    2. Shut down the VM if required.

    3. Go to VM → Snapshot → Snapshot Manager.

    4. Select the snapshot you created.

    5. Click Go To / Restore.

    6. Confirm the operation.

    7. Start the VM.

    8. Verify that the VM has returned to the state saved in the snapshot.

--- Page 3 ---

Part C: Create a VM Clone

   1. Shut down the original VM.

   2. Select the VM in VMware Workstation.

   3. Go to VM → Manage → Clone.

   4. The Clone Virtual Machine Wizard will open.

   5. Select the required snapshot/current state as the cloning source.

   6. Click Next.

   7. Select Create a full clone.

   8. Click Next.

   9. Enter a new name, for example Linux-Clone.

   10. Select the location where you want to save the clone.

   11. Click Finish.

   12. Wait for the cloning process to complete.

   13. Start the cloned VM.

   14. Verify that the cloned VM works independently from the original VM.



To configure and access a shared folder between Host Windows and Guest Windows VM using
VMware Workstation.

VMware Shared Folder allows the Host and Guest operating systems to access the same folder
and share files easily.

Steps

   1. Create a folder named vm-share on the Host Windows machine.

   2. Open VMware Workstation.

   3. Select your Windows Guest VM.

   4. Click Edit Virtual Machine Settings.

   5. Go to Options → Shared Folders.

   6. Select Always enabled.

   7. Click Add.

   8. Click Next.

   9. Select the Host folder vm-share.

   10. Give the folder name as vm-share.

   11. Click Next → Finish.

--- Page 4 ---

12. Click Apply → OK.

   13. Start the Guest Windows VM.

   14. Open File Explorer in the Guest VM.

   15. In the address bar, enter:

\\vmware-host\Shared Folders

   16. Press Enter.

   17. Open the vm-share folder.

   18. Create or copy a file inside it.

   19. Check the same file in the vm-share folder on the Host Windows machine.



Result

The VM snapshot was successfully created and restored, and a separate VM clone was
successfully created also The Shared Folder was successfully configured, and files were accessed
between the Host and Guest Windows machines.
