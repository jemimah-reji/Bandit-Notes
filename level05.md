### Level 5

**Level Goal**  
The password for the next level is stored in the only human-readable file in the `inhere` directory.

**Commands you may need to solve this level:**  
`ls`, `cd`, `cat`, `file`

---

**Explanation of Commands:**

- **file**  
  ➔ Tells you the type of a file (like if it’s text, binary, or something else).

---

**Steps to solve:**

1. Use `ls` to list the files.  
   ➔ You’ll see files named `-file00` to `-file09`.
2. Move into the `inhere` directory:

   ```bash
   cd inhere
   ```

3. **Solution:** Use `file ./*` instead:

   ```bash
   file ./*
   ```

4. Look through the output and find the file that says **ASCII text**.  

5. Read the contents of that file using:

   ```bash
   cat ./-file07
   ```

   ➔ This gives you the password for Level 5.

- **Alternative:** You could also bruteforce it by manually running `cat ./-file00`, `cat ./-file01`, etc. on each file.  
  ➔ But using `file` is way faster and smarter.

---

**Notes:**  
- If a filename starts with a `-`, commands can get confused. Using `./` before the filename tells Linux "this is a file, not a command option."

