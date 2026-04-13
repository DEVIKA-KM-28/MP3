🎵 MP3 Tag Reader & Editor (C Project)
A simple command-line based MP3 metadata reader and editor written in C.
This project allows you to view and modify ID3 tags such as title, artist, album, year, and more from MP3 files.

📌 Features
🔍 View MP3 tag details
✏️ Edit metadata fields:
Title
Artist
Album
Year
Genre
Comment
📖 Help menu for usage guidance
⚡ Lightweight and fast (pure C implementation)

🗂️ Project Structure
.
├── main.c          # Entry point
├── view.c          # View MP3 tags
├── edit.c          # Edit MP3 tags
├── help.c          # Help menu
├── mp3header.h     # Header file
├── sample.mp3      # Sample file for testing
⚙️ Compilation

Use GCC to compile the project:
gcc main.c view.c edit.c help.c -o mp3tool
▶️ Usage
🔹 Show Help
./mp3tool --help
# or
./mp3tool -h
🔹 View MP3 Tags
./mp3tool -v <filename>
🔹 Edit MP3 Tags
./mp3tool -e <option> <new_value> <filename>

Edit Options:
Option	Field
-t	Title
-a	Artist
-A	Album
-y	Year
-c	Comment
-g	Genre
-T	Track

💡 Example
./mp3tool -v sample.mp3
./mp3tool -e -t "New Song Title" sample.mp3

🛠️ Technologies Used
C Programming Language
Standard C Libraries (stdio.h, string.h, etc.)
