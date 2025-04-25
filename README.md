# Metadata-Extraction-using-ExifTool-log2timeline-and-Hidden-Data-Search-using-Steganography-Tools
## NAME: MOHAN S
## REGISTER NUMBER: 212223240094
## AIM:
To extract metadata, perform timeline analysis, and search for hidden data using forensic tools like ExifTool, log2timeline, and steganography detection tools.

## DESIGN STEPS:
### Step 1:
Use exiftool to extract metadata from files such as images, documents, and videos.

### Step 2:
Use log2timeline and plaso to create and analyze event timelines from system logs and file metadata.

### Step 3:
Apply steganography detection tools like steghide, zsteg, or binwalk to uncover hidden data in media files.

## PROGRAM:
Metadata and Timeline Forensics, Steganography Analysis Steps
### STEP 1: INSTALL REQUIRED TOOLS:-
```
sudo apt update
sudo apt install exiftool -y
sudo apt install plaso -y
sudo apt install steghide -y
sudo apt install binwalk -y
```

### STEP 2: EXTRACT METADATA FROM IMAGE:-
```
cd ~/Desktop
```
```
exiftool lion.jpg
```
```
exiftool lion.jpg > abc.txt
```

###  STEP 3: EMBED DATA USING STEGHIDE:-
```
steghide embed -cf /home/kali/Desktop/lion.jpg -ef /home/kali/Desktop/abc.txt
```

###  STEP 4: EXTRACT HIDDEN DATA:-
```
steghide extract -sf /home/kali/Desktop/lion.jpg -p 12 -xf /home/kali/Desktop/output.txt
```

### STEP 5: FILE ANALYSIS USING BINWALK:-
```
binwalk /home/kali/Desktop/lion.jpg
```
```
binwalk -e /home/kali/Desktop/lion.jpg
```


## OUTPUT:
Extracted Metadata, Timeline Events, and Hidden Data Detection Results
```
![EXP5_IMG1](https://github.com/user-attachments/assets/646ef4e9-c683-4296-a348-1b6cbb81e27a)

```
```
![EXP5_IMG2](https://github.com/user-attachments/assets/0e5965b8-44fd-42b3-9cea-77d92d973fd6)

```
## RESULT:
Metadata was successfully extracted, timeline analysis was completed, and hidden data was identified using steganography tools.

