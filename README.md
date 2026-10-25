# alfido-python-task1
Alfido Tech Python Developer Internship - Task 1: Python File Handling & Automation

## About
This program shows how to read and write files (TXT and CSV), automate simple file operations (move, rename, delete), and handle errors with exceptions so the program does not crash.

## What it does
1. setup_demo() creates a folder named file_demo, then writes a text file (sample.txt) and a CSV file (data.csv) with a header row and two task records.
2. automate_files() reads the text file and prints its content.
3. It moves sample.txt to archived_sample.txt (moving to a new name also renames the file).
4. It reads data.csv row by row and prints each task with its status.
5. It deletes the archived text file with os.remove().
6. A final check lists the folder, and only data.csv is left.

## Exception handling
- FileNotFoundError: a file or path does not exist
- PermissionError: the program is not allowed to read or write a file
- Exception: any other unexpected error
- finally: always prints the completion message

## Modules used
os, shutil, csv

## How to run
```
python task1_file_handling.py
```

## Output
```
Created directory: ./file_demo
Sample files created successfully.
Content read: Hello, this is a sample text file for automation demo.
Moved and Renamed sample.txt to archived_sample.txt
Processing: Task_A - Completed
Processing: Task_B - Pending
Deleted archived_sample.txt
File operation sequence completed.
Current files in ./file_demo: ['data.csv']
```

## Repository
https://github.com/alokupadhyay652/alfido-python-task1
