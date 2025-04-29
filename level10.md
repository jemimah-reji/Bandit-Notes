### Level 10

**Level Goal**  
The password for the next level is stored in the file `data.txt`.  
It’s hidden among mostly unreadable content, but the password is:
- One of the **few human-readable strings**
- **Preceded by several `=` characters**

**Commands you may need to solve this level:**  
`cat`, `strings`, `grep`

---

**Explanation of Commands:**

- **strings**  
  ➔ Extracts **human-readable strings** from binary or non-text files.

- **grep**  
  ➔ Filters output by matching patterns.

- **cat**  
  ➔ Shows the full content of a file (used if you wanna scroll manually).

---

**Steps to solve:**

1. Check the contents of `data.txt` using:

   ```bash
   cat data.txt
   ```

   ➔ You’ll see mostly unreadable characters — don’t try to scroll through it manually.

2. Use `strings` to extract only the readable parts:

   ```bash
   strings data.txt
   ```

3. Since Bandit passwords are **32 characters long**, filter with `grep`:

   ```bash
   strings data.txt | grep '[a-zA-Z0-9]\{32\}'
   ```

   ➔ This finds any readable string that’s 32 characters long.

4. Look through the matches — the correct one will be the password.

---

**Notes:**

- `strings` is super useful for digging through messy or binary files.
- Grepping by password length makes it fast and surgical.
