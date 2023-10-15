# How To Git

## 1. Introduction

In this tutorial we will cover the basics of Git by creating a "**repository**" (a collection of tracked files, "repo" for short) with instructions on how to play Tic-Tac-Toe (also called Noughts and Crosses). Don't worry if you don't know how to play the game, the rules will be provided for you. The focus here will be on working with repositories, editing files, and getting comfortable with the basics of Git. Specifically, we will take a basic set of instructions for Tic-Tac-Toe in plain text format, and transform it into a visually appealing guide using a simple formatting language called "Markdown".

> Note: This document was written in Markdown 😃

### What is Git?

Git is what is called a "**version control system**". Version control systems allow multiple people to work on projects without stepping on each other's toes. Git tracks file changes, allows for "**branches**" (alternate universes or timelines) of development, and ensures data integrity (that the saved/tracked data is accurate, reliable, and consistent over time). For developers and collaborative individuals, Git is a valuable skill to learn.

### What You Need to Know First
- Be familiar with using the terminal to enter commands such as `ls` (or `dir` for Windows), `mkdir`, and `touch` or `echo`.
- Be able to navigate to different directories (folders) on your computer using the terminal and the `cd` command.

### What Will You Learn?
By the end of this tutorial, you will:

- Understand basic Git operations and when to use them.
- Be familiar with the structure and syntax of Markdown.
- Have hands-on experience with branching, committing changes, and working with "**remote**" (hosted not on your computer) repositories.
- Know how to undo mistakes in Git, ensuring you can confidently experiment without fear of "breaking" anything.

## 2. How to Install and Configure Git

### How to Install Git

Go [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) and follow the instructions for your operating system

#### You will know your install was a success if:

Open a terminal window and run the command `git --version`. If you see something like "git version 2.25.1" then you have successfully installed Git.

> Note: The version number of Git may be different if you are in the future, and that's OK.

### How to Configure Git
Once installed, it's essential to tell Git who you are. This information is used to track changes in the projects you work on.

Open your terminal or command prompt and enter the following commands:

```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

Replace "Your Name" with your actual name and `"youremail@example.com"` with your email address.

### Section 2 Checkpoint

By now, you should have:

1. Installed Git on your machine.
1. Verified the installation by checking the Git version.
1. Configured Git with your personal details.

## 3. How to Clone a Repo

With Git installed and configured, it's time to dive into our project. Instead of starting from scratch, we're going to use an existing set of Tic-Tac-Toe instructions. This will give you practical experience with one of the most common Git tasks: cloning a repository.

### What is Cloning?
Cloning in Git means creating a local copy (i.e. download) of a remote repository on your machine. This allows you to work on projects, make changes, and then sync those changes back to the remote repository.

### Cloning the Tic-Tac-Toe Instructions
To get our basic version of the Tic-Tac-Toe instructions, follow these steps:

1. Navigate to the directory where you'd like to store the project on your machine using your terminal window.
1. Enter the following command:

```bash
git clone https://github.com/avidrucker/how-to-play-tictactoe.git
```

3. Once the cloning process completes (it may take a few seconds, depending on your Internet connection), you should see a new directory with the name of the repository. This directory contains all the files from the repository.
3. Navigate into the repository directory:

```bash
cd how-to-play-tictactoe/
```

### Section 3 Checkpoint

By now, you should have:

- Cloned the Tic-Tac-Toe instructions repository to your local machine.
- Navigated into the repository directory.

> Note: If you've cloned the repository to the wrong location or forgot to navigate into the cloned directory, don't worry! You can simply move the folder to your desired location using your file system, or delete it and clone again.

## 4. How to Stage Files and Commit File Changes

Now that we have our Tic-Tac-Toe instructions repository on our machine, it's time to start the transformation process. But before we start making changes, we need to understand the current state of our repository. Git provides us with powerful commands to inspect, track, and commit changes.

### How to Inspect a Local Repo

The first thing we want to do is check the status of our repository:

```bash
git status
```

This command will show you any changes made to the repository since the last commit. When you run it now, you'll probably see that everything is up to date and there's nothing to commit.

### Create New File
Let's start by creating a new Markdown file for our improved instructions:

```bash
touch tic-tac-toe.md
```

If you check the status again (git status), you'll see that Git has noticed the new file, but it's currently untracked.

### Track Changes to New File
To start tracking changes to our new file, we use:

```bash
git add tic-tac-toe.md
```

Now, if you check the status, you'll see the file is ready to be committed.

### Commit Changes on New File

After making some improvements to the tic-tac-toe.md file (using any text editor of your choice), you'll want to save these changes in Git. Since we just created the file, for now, let's just commit that change.

```bash
git commit -m "add markdown version of Tic-Tac-Toe instructions"
```

The `-m` "**flag**" lets you add a message to describe the changes you made. It's always a good practice to write a brief and descriptive message so you (or others) can understand the changes at a glance.

> `-m` flag: The `-m` is a specific instruction that you can give to Git when you're using a command like "commit." In this case, it's used with the commit command to add a message that describes what you did in your code changes. So, when you use -m followed by a message, Git knows to associate that message with the changes you're making.
>
> Message: The "message" is just a short note or comment that you write to explain what you did in your code. It helps you and others understand the purpose of your changes. For example, if you fixed a bug or added a new feature, you can use the `-m` flag to include a message like "Fixed a bug in login system" or "Added a new search feature."

### Section 4 Checkpoint

By now, you should have:

- Checked the status of your repository.
- Created a new Markdown file.
- Tracked and committed your changes to the repository.

> Note: If you forget to add a file before committing or skip writing a commit message, Git will remind you. Always read the feedback Git provides in the terminal; it often contains helpful hints and commands.


## Sources

1. What does Git stand for: [stackoverflow question and answer](https://stackoverflow.com/questions/43959748/what-is-the-abbreviation-of-git)
