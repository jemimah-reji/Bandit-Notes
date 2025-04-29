### Level 6

**Level Goal**  
The password for the next level is stored in a file somewhere under the `inhere` directory and has **all** of the following properties:

- Human-readable  
- **Exactly 1033 bytes** in size  
- **Not executable**

**Commands you may need to solve this level:**  
`ls`, `cd`, `cat`, `file`, `du`, `find`

---

**Explanation of Commands:**

- **cd**  
  ➔ Changes the current directory.

- **cat**  
  ➔ Shows the content of a file.

- **find**  
  ➔ Searches for files/folders based on conditions.

---

**Steps to solve:**

1. Move into the `inhere` directory:

   ```bash
   cd inhere
   ```

2. Run the following `find` command to search for a file that:
   - is a regular file (`-type f`)
   - is exactly **1033 bytes** (`-size 1033c`)
   - is **not executable** (`! -executable`)

   ```bash
   find . -type f -size 1033c ! -executable
   ```

3. This returns the path to the correct file, for example:

   ```
   ./maybehere07/.file2
   ```

4. Use `cat` to read it:

   ```bash
   cat ./maybehere07/.file2
   ```

   ➔ That displays the password for Level 6.

---

**Notes:**

- `find` : for narrowing down files based on size, type, and permissions.
- `c` → bytes (e.g. `1033c`)
- `k` → kilobytes (KB)
- `M` → megabytes (MB)
- `G` → gigabytes (GB)
- *(no letter)* → 512-byte blocks

You can also use:
- `+` → greater than  
- `-` → less than  
- (no symbol) → exact size

Example:
```bash
find . -size +1M
```
→ finds files **larger than 1MB**

