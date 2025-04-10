# Mini Project: File and Directory Management Tool
## Project Overview
The **"File and Directory Management Program"** is a bash script that helps users manage files and directories easily. The program is easy to used and work on any system that support bash.

## Key Features
The bash program contains the following features:
1. Displaying Menu <br>
   **Sample Output**:
   ```plaintext
   === Welcome to the File & Directory Tool ===
   1) List files and sub-directories
   2) Backup
   3) Count files
   4) Disk Usage
   5) Search Files
   6) Compress
   7) Exit
   Choose an option: 
   ```
2. List all files and sub-directories with detailed information of a given directory.
   **Sample Output**:
   ```plaintext
   Choose an option: 1
   Listing files and sub-directories:
   Enter the directory path: ../src
   -rwxr-xr-x 1 User 197609  734 Mar 21 23:23 backup.sh
   -rwxr-xr-x 1 User 197609  567 Mar 21 23:08 compress.sh
   -rwxr-xr-x 1 User 197609  501 Mar 22 00:02 count_files.sh
   -rwxr-xr-x 1 User 197609  450 Mar 21 23:13 disk_usage.sh
   -rwxr-xr-x 1 User 197609  369 Mar 21 23:00 list_details.sh
   -rwxr-xr-x 1 User 197609   65 Mar 21 23:14 log_action.sh
   -rwxr-xr-x 1 User 197609 1719 Mar 22 10:43 main.sh
   -rw-r--r-- 1 User 197609 6342 Mar 27 00:50 script.log
   -rwxr-xr-x 1 User 197609  562 Mar 22 10:43 search_file.sh
   Press Enter...
   ```
3. Create backups of individual files and entire directories. <br>
   **Sample Output**:
   ```plaintext
   Choose an option: 2
   Creating backup
   Enter file/directory to backup: compress.sh
   Enter backup destination: ../
   Backup completed to ../
   Press Enter...
   ```
4. Count the number of files in a directory of a given directory. <br>
   **Sample Output**:
   ```plaintext
   Choose an option: 3
   Couting files
   Enter directory to count files: ../src
   Total files: 9
   Press Enter...
   ```
5. Display disk usage of a given directory. <br>
   **Sample Output**:
   ```plaintext
   Choose an option: 4
   Displaying disk usage
   Enter directory to check disk usage: ../src
   38k     ../src
   Press Enter...
   ```
6. Search for a file by name or extension of a given directory. <br>
   **Sample Output**:
   ```plaintext
   Choose an option: 5
   Searchin files
   Enter directory path: ../src
   Enter filename or extension to search (e.g., *.txt): *.sh
   ../src/backup.sh
   ../src/compress.sh
   ../src/count_files.sh
   ../src/disk_usage.sh
   ../src/list_details.sh
   ../src/log_action.sh
   ../src/main.sh
   ../src/search_file.sh
   Press Enter...
   ```
7. Compress the given files or directories. <br>
   **Sample Output**:
   ```plaintext
   Choose an option: 6
   Compressing file or directories
   Enter file or directory to compress: ../src
   Enter output filename (no extension): Source
     adding: ../src/ (260 bytes security) (stored 0%)
     adding: ../src/backup.sh (172 bytes security) (deflated 60%)
     adding: ../src/compress.sh (172 bytes security) (deflated 53%)
     adding: ../src/count_files.sh (172 bytes security) (deflated 48%)
     adding: ../src/disk_usage.sh (172 bytes security) (deflated 51%)
     adding: ../src/list_details.sh (172 bytes security) (deflated 43%)
     adding: ../src/log_action.sh (172 bytes security) (stored 0%)
     adding: ../src/main.sh (172 bytes security) (deflated 73%)
     adding: ../src/script.log (172 bytes security) (deflated 87%)
     adding: ../src/search_file.sh (172 bytes security) (deflated 50%)
   Compressed to Source.zip completed.
   Press Enter
   ```
8. Keep a log file of all actions performed by users in a file called `script.log` in the same directory where you run the program.

## Project Structure
```plaintext
Mini_Project/
├── src/                  # Storing source codes
│   ├── list_details.sh   # 1. List all files and sub-directories
│   ├── backup.sh         # 2. Backup of individual files and entire directories
│   ├── count_files.sh    # 3. Count number of files in a given directory
│   ├── disk_uasge.sh     # 4. Display disk usage of a given directory
│   ├── search_file.sh    # 5. Search for a given file or directory
│   ├── compress.sh       # 6. Compress a given file or directory
│   ├── script.log        # Log file to store all actions of users
│   └── main.sh           # Main file to run all the scripts
└── README.md             # Project documentation
```

## Getting Started
### Requiement
- Windows: Requires Git Bash, You can use Git for GitBash. Ensure you have downloaded Git
```bash
git --version
```
If it displays version of Git. Then it has been installed. If not, install via [Link](https://git-scm.com/)
- Linux/macOS: Pre-installed bash in the machine.
### Installation and Setup
#### Windows 
1. Open Git Bash
2. Clone the repository
```bash
git clone https://github.com/Leangchhay1523/OS_Mini_Project.git
```
3. Navigate to `src` folder in the Project
```bash
cd OS_Mini_Project/src
```
4. Execute the program
```bash
bash main.sh
```
#### Linux/macOS
1. Open terminal
2. Clone the repository
```bash
git clone https://github.com/Leangchhay1523/OS_Mini_Project.git
```
3. Navigate to `src` folder in the Project
```bash
cd OS_Mini_Project/src
```
4. Execute the program
```bash
bash main.sh
```

### Contributor
<div style="display: grid; grid-template-columns: repeat(4, 1fr);">
  <div style="display: flex; justify-content: center; align-items: center; flex-direction: column;">
    <img src="https://github.com/Leangchhay1523.png" alt="Leangchhay Profile" width="50" height="50" style="border-radius: 50%;" />
    <a href="https://github.com/Leangchhay1523">Leangchhay1523</a>
  </div>
  <div style="display: flex; justify-content: center; align-items: center; flex-direction: column;">
    <img src="https://github.com/Sitharath-s.png" alt="Sitharath-S's Profile" width="50" height="50" style="border-radius: 50%;" />
    <a href="https://github.com/Sitharath-s">Sitharath-S</a>
  </div>
  <div style="display: flex; justify-content: center; align-items: center; flex-direction: column;">
    <img src="https://github.com/PunleuTY.png" alt="PunleuTY's Profile" width="50" height="50" style="border-radius: 50%;" />
    <a href="https://github.com/PunleuTY">PunleuTY</a>
  </div>
   <div style="display: flex; justify-content: center; align-items: center; flex-direction: column;">
    <img src="https://github.com/Mey15.png" alt="Mey15's Profile" width="50" height="50" style="border-radius: 50%;" />
    <a href="https://github.com/Mey15">Mey15</a>
  </div>
</div>
