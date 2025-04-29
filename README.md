# Bandit Notes

This repo contains my notes and solutions for the **Bandit wargame** from [OverTheWire](https://overthewire.org/wargames/bandit/).

The Bandit game is designed to teach the basics of Linux commands, file system navigation, and remote server access.

---

## How to Start

1. **Install SSH**  
   Make sure you have SSH installed (you probably already do if you're on Linux or Mac. Windows users can use Command Prompt, Git Bash, or WSL).

2. **Login to Bandit**  
   To connect to the Bandit server, open your terminal and type:

   ```bash
   ssh bandit0@bandit.labs.overthewire.org -p 2220
   ```

   - Username: `bandit0`
   - Host: `bandit.labs.overthewire.org`
   - Port: `2220`
   - Password: (Provided on the Bandit website for Level 0)

---

## How to Progress to the Next Level

- After solving a level, you will find the **password** for the next level.
- Use that password to **log in** to the next user.
- Example to move to Level 1:

  ```bash
  ssh bandit1@bandit.labs.overthewire.org -p 2220
  ```

  (And paste the new password when asked.)

- **TIP:** Save passwords as you go! They are not saved automatically.

---

## Notes Organization

Each level has:
- A description of the level goal
- Commands used
- Step-by-step solution
- Any tips or notes for tricky parts

---

## Why I'm Doing This

- Practice Linux basics 
- Build cybersecurity skills 
- Keep a record of my journey 
- Help others who might be starting out 

---
## Disclaimer

These solutions are for educational purposes only. Please don’t just copy-paste — take time to understand the commands and concepts. All content here is based on my personal walkthrough of the OverTheWire Bandit game.
