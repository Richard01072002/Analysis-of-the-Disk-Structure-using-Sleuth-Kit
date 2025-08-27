# Analysis-of-the-Disk-Structure-using-Sleuth-Kit
### Name - Richardson a
### Reg. No. - 212222233005
## AIM:
To analyze the disk structure of a given disk image using Sleuth Kit tools in Kali Linux.

## DESIGN STEPS:
### Step 1:
Obtain or create a disk image file (e.g., disk.dd) to analyze. Open the terminal in Kali Linux.

### Step 2:
Use Sleuth Kit tools like mmls, fsstat, and fls to examine the partition layout, file system details, and file listing.

### Step 3:
Interpret the output of the tools to understand the disk structure, including partitions, sectors, and files.

## PROGRAM:

### Sleuth Kit Disk Analysis Commands

#### Create a Sample Disk Image (for Testing)

#### Let’s create a 10MB blank disk image and simulate file system activity:

```
cd ~/Downloads
```

#### Step 1: Create an empty disk image

```
dd if=/dev/zero of=disk.dd bs=1M count=10
```

#### Step 2: Format it with a file system (like FAT32)

```
mkfs.vfat disk.dd
```


## OUTPUT:
<img width="315" height="88" alt="Screenshot 2025-08-28 at 2 25 38 AM" src="https://github.com/user-attachments/assets/d81f5217-a526-4ee7-b2bc-903d610280ca" />

## Create Disk
<img width="1110" height="416" alt="image" src="https://github.com/user-attachments/assets/19c09a8d-c258-43cc-95cc-ff84220f8e37" />



## mmls

```
mmls disk.dd
```

## fls

```
fls -f fat -o 0 disk.dd
```
<img width="811" height="499" alt="Screenshot 2025-08-28 at 2 26 59 AM" src="https://github.com/user-attachments/assets/43da440f-78f9-44a4-bf89-aa0c27d02082" />




## RESULT:
The analysis was performed successfully using Sleuth Kit, and the disk structure was understood in detail.
