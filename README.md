PART 1 – Git Setup (Do this once)
git --version
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --global --list
PART 2 – Create the Project folder
mkdir Gitlab
cd Gitlab
git init
ls -a
git status
PART 3 – Create the File
Method A: touch (create an empty file)
touch program1.txt
git status

Method B: nano (create and edit the file directly)
nano program1.txt
Type:
Student Name: Rahul
USN: 101
Branch: CSE-CY	

Save in nano: Ctrl + O → Enter
Exit nano: Ctrl + X
Note: If you use touch first, you can later run nano student.txt to edit the empty file.
 
Method C: notepad
notepad program1.txt

PART 4 – Check the New File
git status

PART 5 – Stage the File                                                                                      git restore --staged marks.py
git add program1.txt
git status
PART 6 – First Commit
git commit -m "VERSION 1"

PART 7 – View Commit History
git log
git log --oneline
git show HEAD
PART 8 – Modify the File
nano program1.txt
Add: Semester: 3
Save: Ctrl + O → Enter
Exit: Ctrl + X
Symbol	Meaning
---	Old/original version
+++	New/current version
-	A line was removed
+	A line was added
PART 9 – See What Changed
git status									
git diff                        
PART 10 – Stage and Review the Change
git add program1.txt
               
PART 11 – Commit the Modification
git commit -m "VERSION 2"

PART 12 – Demonstrate git commit -am
Modify program1.txt         again using nano program1.txt
git commit -am "Update semester"

