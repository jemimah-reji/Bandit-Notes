### Level 7

**Level Goal**  
The password for the next level is stored somewhere on the server and has **all** of the following properties:

- Owned by **user `bandit7`**
- Owned by **group `bandit6`**
- Exactly **33 bytes** in size

**Commands you may need to solve this level:**  
`find`, `cat`

---

**Explanation of Commands:**

- **find**  
  ➔ Searches for files and folders based on conditions.

- **cat**  
  ➔ Shows the content of a file.

---

**Steps to solve:**

1. Since the file could be **anywhere** on the server, start your search from the root `/` directory.
2. Use the `find` command with these options:
   - Search from `/`
   - Look for files owned by `bandit7`
   - Look for files in group `bandit6`
   - Look for files exactly **33 bytes** in size

   ```bash
   find / -user bandit7 -group bandit6 -size 33c 2>/dev/null
   ```

   - `2>/dev/null` is used to **hide permission errors** you don't care about.

3. `find` will show a path 

4. Use `cat` to read the file:

   ```bash
   cat /filepath
   ```

   ➔ This will display the password for Level 7.

