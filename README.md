# Simple Git Tutorial: Tic-Tac-Toe Guide

## 1. Setup and Introduction
- Git is a tool to track changes in code. It's like a supercharged 'save' feature.
- We'll make a nice-looking Tic-Tac-Toe guide using it.
- Prerequisites: Familiarity with basic terminal or command prompt commands.

## 2. Install and Setup Git
- Install: [Download Git here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and follow the instructions.
- Setup: Tell Git who you are:
```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

## 3. Get the Tic-Tac-Toe Instructions
- Go to [Tic-Tac-Toe instructions](https://github.com/avidrucker/how-to-play-tictactoe).
- Click "Fork" to get your own copy on GitHub.

## 4. Download Your Copy
- On your GitHub fork, click "code" > copy the link.
- On your computer:

```bash
git clone YOUR_LINK_HERE
cd how-to-play-tictactoe/
```

## 5. Make a Better Tic-Tac-Toe Guide
- Make a new file: `touch tic-tac-toe.md`
- Use any text editor to write a guide in this file.
- Save your changes in Git:
```bash
git add tic-tac-toe.md
git commit -m "Created a new Tic-Tac-Toe guide."
```

## 6. Update Your GitHub Copy
- To save your local changes online:
```bash
git push
```

## 7. Oops! Made a Mistake?
- Git's got you covered. Use commands like `git log`, `git reset`, and others to backtrack.

## 8. Ignore Unnecessary Files
- Some files (like temporary ones) don't need to be in Git. Use a .gitignore file to list them.
