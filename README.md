<h1 align = "center">𐔌 .⋮ NotesDump  .ᐟ  ֹ   ₊ ꒱</h1>
<h3 align = "center">Your console-based short notes dump.</h3>
<p align = "center">
<b>CS 2106 </b> <br/>
Agdon, Fatima Marie P. <br/>
Pastrana, Jei Q. <br/>
Perez, Renz Marrion O.
</p>

## ‧₊˚ ┊ Overview
NotesDump is a console-based Java application allowing users to manage note entries directly through the terminal.
<br/><br/>
It demonstrates the practical use of Object-oriented Programming (OOP) concepts such as encapsulation, inheritance, polymorphism, and abstraction, alongside proper file handling and modular design.
<br/>
### Users can:
✏️ Add a new entry<br/>
📔 View all entries<br/>
✍🏻 Modify or delete specific entries<br/>
📑 Insert an entry at a certain index

### Note Entry Storage
💾 All entries are stored in a plain text file.

## ‧₊˚ ┊ Project Structure
```
📂 src/
└── 📂 diaryapp/
    ├── ☕ Main.java          
    ├── ☕ Diary.java
    └── ☕ FileHandler.java
```
- `Main.java` - Entry point of the program, containing the menu and handles user interactions.
- `Diary.java` - Handles the diary operations (CRUD)
- `FileHandler.java` - Handles file creation, reading, writing, and appending.
### How to Run the Program
Open your terminal in the `src/` folder and run:
```
javac diaryapp/*.java
```
Run the program using:
```
java diaryapp.Main
```
## ‧₊˚ ┊ Features
1. **Add Entry.** Create a new diary entry with timestamp.
2. **View Entries.** Display all saved entries with numbering.
3. **Modify Entry.** Edit any existing note by selecting its number
4. **Delete Entry.** Remove a specific entry permanently.
5. **Insert Entry.** Add a note at any position in the list.

## ‧₊˚ ┊ Object-oriented Principles
### 💊 Encapsulation
Encapsulation was applied through class design and private fields. For instance, in `Diary`, the `filepath` variable is private and can only be accessed through the class's own methods such as, `addEntry()`, `viewEntries()`, etc.

This ensures that data and operations on it are bundled together and protected from unauthorized modification.

### 💡 Abstraction
Abstraction was implemented when the `FileHandler` class abstracts file operations like reading, writing, and appending. The `Diary` class doesn't need to know how file handling works, for it just calls methods like `FileHandler.appendLine()` or `FileHandler.readAllLines()`.

This hides low-level complexity and keeps the main logic clean.

### 🧬 Inheritance
Inheritance was not heavily used in the program, however, its structure is ready for extension.
For instance, if a subclass like for diary is to be created, it could inherit from `Diary` and override some methods like `addEntry()` and `viewEntries()`.

This shows potential for code reuse and expansion without rewriting existing logic.

### 🎭 Polymorphism
The `switch` expression in `Main.java` demonstrates method-level polymorphism, the same action (`diary.[action]`) calls different behaviors depending on user choice.

Also, if a subclass of `Diary` overrides a method, for instance `addEntry()`, the program could dynamically call the correct version at runtime, enabling flexible behavior.

## ‧₊˚ ┊ Example Output
```
--- NOTES DIARY ---
1. Add an entry
2. View all entries
3. Modify an entry
4. Delete an entry
5. Insert an entry
6. Exit
Enter your choice: 1
Enter your note. (Press x to cancel): Had coffee while coding!
Entry added.
Press Enter to continue...

```

##  ‧₊˚ ┊ notes.txt Snippet
```
2025-11-09 11:10:16 | Woah-oh bakit ba ganito?
2025-11-09 11:10:27 | Palaging bumabalik sa'yo?
2025-11-09 11:10:43 | Woah-oh, litong-lito
2025-11-09 11:10:55 | na ang puso ko~~~
2025-11-09 11:11:18 | Paikot-ikot, nahihilo
2025-11-09 11:11:26 | Gulong-gulo ang isipan ko
2025-11-09 11:11:51 | Handa ng magpasalo
2025-11-09 11:11:58 | Basta ikaw ang kasalo
2025-11-09 11:12:08 | Hanggang sa dulo ng mundo
2025-11-09 11:12:22 | Paikot-ikot na lang sa'yo
2025-11-09 11:12:33 | Sana'y pakinggan mo 'ko
2025-11-09 11:12:54 | Dahil handa na akong
2025-11-09 11:13:00 | magpasalo
2025-11-09 11:13:11 | Basta ikaw ang kasalo <3
```

##  ‧₊˚ ┊ Contributors
| &nbsp; | Name | Duty/Responsibility |
|--------|------|---------------------|
| <img src="static/marieemoiselle.JPG" width="100" height="100"> | Fatima Marie P. Agdon, MSCS | Project Leader/ System Architect |
| <img src="static/jeisquared.jpg" width="100" height="100"> | Jei Q. Pastrana, MSIT | File Handling Specialist |
| <img src="static/renzmarrion.jpg" width="100" height="100"> | Renz Marrion O. Perez | Feature Developer |

##  ‧₊˚ ┊ Acknowledgment
We sincerely express our gratitude to our instructor for the guidance and support provided throughout the completion of this project. We also extend our appreciation to our classmates and peers for their cooperation and encouragement during the development process.

---
<small>
<b>DISCLAIMER</b><br/>
This project and its contents are provided for example and learning purposes only. Students are encouraged to use it as a reference and not copy it in its entirety.</small>