## Linux Host

This section show how to install an operating system to your B2260 using the SD Card method on a Linux host computer.
***

- **Step 1**: Prepare MicroSD card
- **Step 2**: Find SD Card Device name
- **Step 3**: Recall Download Location
- **Step 4**: Unzip _SD Card Install Image_
- **Step 5**: Go to directory with _SD Card Install Image_ folder using Terminal
- **Step 6**: Locate SD Card Install Image
- **Step 7**: Install Image onto SD Card
- **Step 8**: Prepare B2260 with SD card

***

####**Step 1**: Prepare MicroSD card

- Ensure data from mircoSD card is backed up
- Everything on microSD card will be lost by the end of this procedure.

####**Step 2**: Find SD Card Device name

- Use host computer
- Open "Terminal" application
- Remove SD card from host computer and run the following command:
```shell
$ lsblk
```
- Note all recognized disk names
- **Insert SD card** and run the following command (again):
```shell
$ lsblk
```
- Note the newly recognized disk. This will be your SD card.
- **Remember** your SD card device name, it will be needed in **Step 7**.

####**Step 3**: Recall Download Location

- Locate SD card install file from Downloads page.
- This file will be needed for the next step.

####**Step 4**: Unzip _SD Card Install Image_

- When unzipped, you will have a file:
   - Install Image (.img)

####**Step 5**: Go to directory with _SD Card Install Image_ folder using Terminal

- Use host computer
- Open "Terminal" application
- `cd` to the directory with your unzipped **SD Card Install Image**

```shell
$ cd <extraction directory>

#Example:
#<extraction directory> = /home/YourUserName/Downloads
#For this example we assume the "SD Card Install Image" is in the Downloads folder.
$ cd /home/YourUserName/Downloads
```

####**Step 6**: Locate SD Card Install Image

- Make sure you are in the extraction directory
- Locate your preferred image file (latest one maybe the best option)

**Unzipped SD Card download will be a file.** Type `ls` from command line :

```shell
ls

#output
b2260-jessie_developer_YYYYMMDD-X.img
```
**Checklist:**

- SD card inserted into host computer
- Recall SD Card device name from **Step 2**
- Using the Terminal to copy b2260-jessie_developer_YYYYMMDD-X.img image file into SD card by ###**Step 8**: Prepare B2260 with SD card

- Make sure B2260 is unplugged from power
- Connect an HDMI monitor to the B2260 with an HDMI cable, and power on the monitor
- Plug a USB keyboard and/or mouse into either of the two USB connectors on the B2260
- Insert the microSD card into the B2260
- Plug power adaptor into B2260, wait for board to boot up.

**Congratulations! You are now booting your newly installed operating system directly from SD card on the B2260!**
