# Making a Bootable USB Drive from an ISO

Creating a bootable USB drive is one of the easiest ways to install or reinstall an operating system. Whether you're setting up a new computer, recovering a system, or performing a clean installation, the process is straightforward.

## Requirements

Before you begin, make sure you have the following:

* An ISO file of the operating system you want to install.
* A USB flash drive.

  * The required capacity depends on the operating system. An 8 GB drive is enough for most Windows and Linux distributions, while some operating systems may require more.
* A USB creation tool such as:

  * **Rufus** (Recommended)
  * **Ventoy**
  * **Microsoft Media Creation Tool** (Windows only)

> **Warning**
> This process will erase all data on the selected USB drive. Back up any important files before continuing.

---

## Creating a Bootable USB with Rufus

### Step 1: Download Rufus

Download the latest version of Rufus from the official website:

https://rufus.ie/

Rufus is portable, so it does not require installation.

### Step 2: Launch Rufus

Open **Rufus** and insert your USB flash drive.

### Step 3: Configure Rufus

Configure the following options:

* **Device:** Select your USB drive.
* **Boot selection:** Click **Select** and choose your ISO file.
* **Partition scheme:** Choose **GPT** for most modern computers.

  * Use **MBR** only if you're installing on an older system that does not support UEFI.
* **Target system:** Choose **UEFI**.

  * Select **BIOS (Legacy)** only if your computer requires it.

> **Tip**
> GPT + UEFI is the recommended configuration for nearly all modern Windows 10 and Windows 11 computers.

Leave the remaining settings at their default values unless you have a specific reason to change them.

### Step 4: Start the Process

Click **Start**.

Rufus will display a warning that all data on the USB drive will be deleted.

Select **OK** to continue.

Wait for Rufus to finish writing the ISO to the USB drive.

---

## Done!

Your bootable USB drive is now ready to use.

Restart your computer, boot from the USB drive, and follow the operating system's installation process.

---

## Additional Resources

If you're unsure how to boot from a USB drive or install your operating system, check out the other documentation and tutorials in this repository.

Thanks for reading! If this guide helped you, consider starring the repository and checking back for more IT-related documentation and tutorials.
