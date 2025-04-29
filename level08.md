### Level 8

**Level Goal**  
The password for the next level is stored in the file `data.txt` next to the word **millionth**.

**Commands you may need to solve this level:**  
`ls`, `cat`, `grep`

---

**Explanation of Commands:**

- **ls**  
  ➔ Lists the files and folders in the current directory.

- **cat**  
  ➔ Shows the content of a file.

- **grep**  
  ➔ Searches for lines that match a specific word or pattern.

---

**Steps to solve:**

1. After logging into `bandit7`, list the files:

   ```bash
   ls
   ```

   ➔ You will see a file called `data.txt`.

2. Use `grep` to search for any line containing the word **millionth**:

   ```bash
   grep "millionth" data.txt
   ```

3. The text next to `millionth` is the password.

---

**Notes:**
- You can also make `grep` even stricter by using:

  ```bash
  grep "^millionth" data.txt
  ```

  ➔ `^` means "line starts with", so you only match lines starting with `millionth`.
