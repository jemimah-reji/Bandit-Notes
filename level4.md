### Level 4

**Level Goal**  
The password for the next level is stored in a hidden file in the `inhere` directory.

**Commands you may need to solve this level:**  
`ls`, `cd`, `cat`, `find`

---

**Explanation of Commands:**

- **ls**  
  ➔ Lists the files and folders in the current directory.

- **cd**  
  ➔ Changes the current directory.

- **cat**  
  ➔ Shows the content of a file.

- **find**  
  ➔ Searches for files and folders.

---

**Steps to solve:**

1. Use `ls` to see the contents of the current directory.  
   ➔ You’ll see a folder named `inhere`.
2. Go into the directory:

   ```bash
   cd inhere
   ```

3. If you just run `ls`, you’ll see nothing. That’s because the file is **hidden**.
   To see hidden files, you can use:

   ```bash
   find
   ```

4. It will show a file like `./...Hiding-From-You`.  
   ➔ It has **three dots** in the name.

5. Use `cat` to read it:

   ```bash
   cat ./...Hiding-From-You
   ```

   ➔ This will display the password for Level 4.

---

**Notes:**  
- Hidden files in Linux start with a dot `.`  
- Files with multiple dots like `...filename` still count as hidden.
- `find` is super useful to discover hidden or weirdly named files.
