### Level 3

**Level Goal**  
The password for the next level is stored in a file called `spaces in this filename` located in the home directory.

**Commands you may need to solve this level:**  
`ls`, `cat`

---

**Explanation of Commands:**

- **ls**  
  ➔ Lists the files and folders in the current directory.

- **cat**  
  ➔ Shows the content of a file.

---

**Steps to solve:**

1. Use `ls` to list the files.  
   ➔ You’ll see a file named `spaces in this filename`.
2. Since the filename has **spaces**, you can't just type it normally.  
   You need to either:
   
   ```bash
   cat spaces\ in\ this\ filename
   ```
   (escape each space with `\`)

   ➔ This will display the password for Level 3.

---

**Notes:**  
- In Linux, spaces are treated as separators between commands and arguments.
- `\` escapes the space, telling the terminal "this is still part of the same filename."

**Reference:**  
[StackExchange: Is space not allowed in a filename?](https://unix.stackexchange.com/questions/148043/is-space-not-allowed-in-a-filename)

