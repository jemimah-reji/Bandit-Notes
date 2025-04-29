### Level 2

**Level Goal**  
The password for the next level is stored in a file called `-` located in the home directory.

**Commands you may need to solve this level:**  
`ls`, `cat`, `cd` , `cat` , `file` , `du` , `find`

---

**Explanation of Commands:**

- **ls**  
  ➔ Lists the files and folders in the current directory.

- **cat**  
  ➔ Shows the content of a file.

---

**Steps to solve:**

1. Use `ls` to list the files.  
   ➔ You’ll see a file named `-`.
2. You can't use a normal `cat -` because `-` is a special symbol in Linux.  
   So instead, use either:

   ```bash
   cat ./-
   ```
   or
   ```bash
   cat < -
   ```

   ➔ This will display the password for Level 2.

---

**Notes:**  
- `./` tells the system this file right here instead of treating `-` like special input.
- `<` redirects input from the file named `-`.

**Reference:**  
[StackOverflow: How to open a dashed filename using terminal](https://stackoverflow.com/questions/42187323/how-to-open-a-dashed-filename-using-terminal)
