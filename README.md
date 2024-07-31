## Updates:

I will try to capture my 3DS properly at some point to add pictures, and I will also try to customize the texts better.


# What you need

1. you need an SD card with at least 2 GB of storage space. Ideally, it should have more than 2 GB, preferably 32 GB.
2. a 3DS or 2DS, whether Old, New, XL or normal.
3. a PC, laptop or similar to change or add data to the SD card.

# SD Card Preparation

## Windows

1. Download [Fat32 Format](http://ridgecrop.co.uk/index.htm?guiformat.htm).
2. Run "guiformat.exe".
3. Select your SD card (e.g., "D:").
4. If your SD card is 32 GB or larger, select "32768" for "allocated unit size" so that the 3DS can recognize the SD card. (Some SD cards, especially older ones, might still not be recognized if they are larger than 32 GB.)

## MacOS

1. Open "Disk Utility".
2. Right-click on the SD card and select "Erase". Format it as Fat32 (it may be displayed as "MS-DOS (FAT)").
3. Then select "Erase".

## Linux

1. Open the "Disks" app.
2. Select the disk, then click on the gear icon or right-click and choose "Format".
3. Choose "Fat32" as the file system type (you may need to go to "Other" or "Additional" to select Fat32).

# 3DS Preparation

1. Insert the SD card into your 3DS and wait for the data to be created on the SD Card.
2. Go to Mii Maker and wait for the data to be created if it does not already exist.
3. Go to the System Settings, select "General Settings" and then go right to `System Update' (you should be at v.11.17.0-50; the letter behind the number only indicates the region).4
4. In the system settings, go to "Data Management". Remove your SD card and insert it into your PC (You should leave your 3DS turned on).

# SD Card Setup

1. Download the 3DS Modding Setup data from the "Downloads.txt" file and unpack it.
2. Install Python from the official website.
3. Place the `dbs` folder in the Nintendo 3DS folder, in the two long-digit subfolders where the folder "extdata" is also located.
4. Copy all data from the `SD` directory directly to the root directory of the SD card.
5. Pack the SD card into the 3DS.

# Prepare payload

1. On your 3DS, in the system settings, go to Data Management (where we should already be), select "Software" and then "Reset" (your data will not be deleted).
2. Then remove your SD card and put it in your PC.

# Insert Payload

1. Open the file `mset9.bat` (in Windows), `mseset9.py` (on Windows and Linux) or `msets9.command` (in macOS).
2. In the script, choose whether you have a New 3DS or Old 3DS.
3. Then choose `Inject MSET9 Payload`.
4. Insert the SD card back into the 3DS (leave the 3DS on).

# Load Payload

1. Go to Data Management on the 3DS and select "Additional Data".
2. Enter the key combination shown above.
3. After the 3DS is restarted, turn it off.

# Remove Payload

1. Put the SD card back into your PC.
2. Open the mset9 script again.
3. Select your 3DS version again.
4. Select "Remove MSET9 Payload".
5. Put your SD card back into the 3DS.

# Enable "Enable loading external FIRMs and modules" and "Enable Game patching" to install mods

1. Press the "Select" button before starting to enter the "Luma3DS Firmware" configuration mode.
2. Place a hook on the options listed in this header.
3. Then restart the 3DS.

# Dump DSP Firmware

1. Simultaneously press "L + Control Cross Down + Y".
2. Choose `Miscellaneous Options`.
3. Then choose `Dump DSP Firmware` and `Nullify User Time Offset`.

# Install Homebrews and additional software

1. Press the "Start" button before starting the 3DS to boot into the "GodMode9".
2. Then select the "Home" button.
3. Select `Scripts`.
4. Then choose `Finalize` (Backupt also automatically the NAND).
5. Just press "A" and then the key combination that appears on the bottom screen.
6. Restart your 3DS.
7. Open "FBI".
8. Go to "SD".
9. Then go to "cias".
10. Select "current directory".
11. Select "Install and Delete all CIAs".

# Backup of the NAND (Manuell)

1. Restart GodMode9 when starting the 3DS.
2. Press the "Home" button.
3. Select `Scripts`.
4. Then choose `GM9Megascript`.
5. Finally, choose `Backup Options`.
6. Choose `SysNAND`.
7. Turn off the 3DS.
8. Plug the SD card into your PC.
9. Go to the folder "gm9" on the SD card and then to the "out" folder.
10. Save the files (with the suffix) `.bin`, '.bin.sha` and `.exefs` to a backup folder.
