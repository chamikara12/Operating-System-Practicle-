# Day 01

# System Setup and Info Scripts

This repository contains two simple scripts:

1. A shell script to create a directory structure based on criteria and standards.
2. A Windows batch script to display system information like username, Windows version, and current date/time.

---

## 1. Directory Structure Script

This shell script creates a series of folders for organizing criteria and their respective standards. Each `criteria_x` folder contains several `standard_y` subfolders.

### Structure Created:
```
criteria_1/
  ├── standard_1/
  └── standard_2/
criteria_2/
  ├── standard_1/
  └── standard_2/
criteria_3/
  ├── standard_1/
  ├── standard_2/
  └── standard_3/
criteria_4/
  ├── standard_1/
  ├── standard_2/
  └── standard_3/
criteria_5/
  ├── standard_1/
  ├── standard_2/
  └── standard_3/
criteria_6/
  ├── standard_1/
  ├── standard_2/
  └── standard_3/
```

### Sample Shell Script
```sh
mkdir criteria_1
cd criteria_1
mkdir standard_1 standard_2
cd ..

mkdir criteria_2
cd criteria_2
mkdir standard_1 standard_2
cd ..

mkdir criteria_3
cd criteria_3
mkdir standard_1 standard_2 standard_3
cd ..

mkdir criteria_4
cd criteria_4
mkdir standard_1 standard_2 standard_3
cd ..

mkdir criteria_5
cd criteria_5
mkdir standard_1 standard_2 standard_3
cd ..

mkdir criteria_6
cd criteria_6
mkdir standard_1 standard_2 standard_3
```

---

## 2. Windows Batch Script

This script displays basic system information, such as the username and Windows version, and prompts the user to check or change the date and time.

### Sample Batch Script
```bat
:: 2021ICT29

:: Disable command echoing in the result
@echo off

:: Display the current username
echo Username: %USERNAME%

:: Display the Windows version
echo Windows Version:
ver

:: Display the current system date and prompt the user to change it
echo Current system date:
date

:: Display the current system time and prompt the user to change it
echo Current system time:
time

:: Pause the script execution until the user presses a key
pause
```
![Screenshot (8)](https://github.com/user-attachments/assets/4268dad5-9444-4dae-bb2a-27b68c69cc8a)


> 💡 Tip: If you only want to **display** date and time without prompting the user to change them, use:
> ```bat
> echo %DATE%
> echo %TIME%
> ```

---
