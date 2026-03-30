# 🐧 Linux File Operations Practice

## 📅 Topic
File creation, movement, deletion, and path understanding in Linux

---

## 📁 1. Create Multiple Files Using Brace Expansion

```bash
touch devopsfile{1..10}.txt
🔍 Output
devopsfile1.txt  devopsfile2.txt  ... devopsfile10.txt

👉 Creates 10 empty files in one command

⏱️ 2. Create Files with Timestamp
touch file_$(date +%Y%m%d_%H%M%S).txt
🔍 Example Output
file_20260330_101530.txt

👉 Useful for logs and backups

📦 3. Copy Files (cp)
Copy file
cp devopsfile1.txt backup.txt
Copy multiple files
cp devopsfile{1..3}.txt /tmp/
🚚 4. Move / Rename Files (mv)
Rename file
mv devopsfile1.txt newfile.txt
Move file
mv newfile.txt /tmp/
📍 5. Absolute vs Relative Path
🔹 Absolute Path

👉 Full path from root /

cd /home/ubuntu
🔹 Relative Path

👉 Path from current directory

cd ../tmp
❌ 6. Remove Files
Remove single file
rm devopsfile1.txt
Force remove (ignore errors)
rm -f devopsfile2.txt
Remove directory recursively
rm -rf testdir/

👉 Deletes directory + all contents

⚠️ Dangerous Command
rm -rf *

👉 Deletes EVERYTHING in current directory

🚨 Important Notes
-r → recursive (delete folders)
-f → force (no confirmation)
Always check before running dangerous commands
🧠 Key Learnings
Brace expansion saves time
Timestamp helps in unique file naming
cp copies, mv moves/renames
Absolute path = full path
Relative path = current location based
rm -rf * is risky (use carefully)
🧑‍💻 Author

Tulasi Kumar Sahu
DevOps Engineer | Linux Learner


---

If you want next:
👉 I can convert this into a **real project (log rotation + backup automation script)**  
👉 Or give you **Linux interview questions from this topic (Amazon level)** 🔥
