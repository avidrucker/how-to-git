# Intro Git How-To: Creating a README File

## 1. Introduction
- Git is a version control system that helps you track changes in files.
- In this tutorial, we'll create a simple README file using Git.
- No prior Git experience required.

## 2. Install Git
- Download and install Git from [here](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).
- Open your terminal or command prompt.
- Configure Git with your name and email:
  ```bash
  git config --global user.name "Your Name"
  git config --global user.email "youremail@example.com"
  ```

## 3. Create a New Git Repository
- Again in your terminal or command prompt, navigate to the folder where you want to create your project (make sure this folder is only for your project, and contains nothing else)
- Initialize a new Git repository:
  ```bash
  git init
  ```

## 4. Create Your README File
- Create a new file named `README.md` in your project folder.
- Edit `README.md` using a text editor and paste the following Markdown content:
  ```
  # Project Title

  A brief description of your project.

  ## Image
  ![Image Description](image_link_here)

  ## Link
  [Click here](your_link_here)

  ## List
  - Item 1
  - Item 2
  - Item 3

  ## Headings
  ### Subheading 1
  ### Subheading 2
  ```

## 5. Track Changes with Git
- Check the status of your Git repository:
  ```bash
  git status
  ```
- Add your `README.md` to the staging area:
  ```bash
  git add README.md
  ```
- Commit your changes:
  ```bash
  git commit -m "Added README file"
  ```

## 6. Recap
- You've learned how to initialize a Git repository, check the status, stage files, and commit changes.
- These are the foundational commands of Git, essential for basic version control.
