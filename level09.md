### Level 9

**Level Goal**  
The password for the next level is stored in the file `data.txt` and is the **only line of text that occurs once**.

**Commands you may need to solve this level:**  
`sort`, `uniq`, `cut`, `cat`

---

**Explanation of Commands:**

- **cat**  
  ➔ Shows the full contents of a file.

- **sort**  
  ➔ Sorts the lines of text alphabetically or numerically.

- **uniq**  
  ➔ Filters out repeated lines from sorted input.  
  ➔ `-u` flag only shows lines that appear **once**.

- **cut**  
  ➔ Extracts specific columns or fields from lines.

---

**Steps to solve:**

1. Looking for a line that shows up **only once** in the file.

2. Use `sort` + `uniq -u` to isolate that line:

   ```bash
   sort data.txt | uniq -u
   ```

   ➔ This shows all lines that appear **only once**.

3. Once you find the unique line, that’s your password.

---

**Reference:**  
- [GeeksForGeeks: `uniq` Command in Linux](https://www.geeksforgeeks.org/uniq-command-in-linux-with-examples/)
