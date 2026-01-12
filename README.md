# CS101: Data Structures

Activity 01: Installing Essential Tools and Solving the Maze

## Assigned: Wednesday, 14th January 2026

## Due: Friday, 16th September 2025, by 11:00am (end of class) via GitHub

![Maze Example](graphics/logo.png)

## Table of contents
- [CS101: Data Structures](#cs101-data-structures)
  - [Assigned: Wednesday, 14th January 2026](#assigned-wednesday-14th-january-2026)
  - [Due: Friday, 16th September 2025, by 11:00am (end of class) via GitHub](#due-friday-16th-september-2025-by-1100am-end-of-class-via-github)
  - [Table of contents](#table-of-contents)
  - [Deliverables](#deliverables)
  - [Project Goals](#project-goals)
  - [Part 1: Installing Commonly Used Tools](#part-1-installing-commonly-used-tools)
    - [VSCode](#vscode)
    - [Git Setup](#git-setup)
      - [Download and Install Git](#download-and-install-git)
      - [Create Your Free Account](#create-your-free-account)
      - [Set Up Your GitHub Profile](#set-up-your-github-profile)
      - [Set up your SSH Keys for use with GitHub](#set-up-your-ssh-keys-for-use-with-github)
      - [Generate the SSH Key Pair](#generate-the-ssh-key-pair)
      - [Add the Public Key to GitHub](#add-the-public-key-to-github)
    - [Python3: A programming language](#python3-a-programming-language)
    - [GatorGrade](#gatorgrade)
    - [Checking Your Work](#checking-your-work)
  - [Part 2: Maze Solving and Instruction Exchange](#part-2-maze-solving-and-instruction-exchange)
  - [Reflection Questions](#reflection-questions)

## Deliverables

You are to complete and push to your repository the completed File: `writing/reflection.md`. This writing contains a reflection, and your responses to some questions (contained in the document).

## Project Goals

+ To learn how to install and configure essential software for coding.
+ To practice giving and following precise instructions.
+ To develop skills in collaboration and critical analysis.

---

## Part 1: Installing Commonly Used Tools

In this part of the activity, you will install three commonly used tools for programming and software development: Visual Studio Code (VSCode), Git, and Python3. These tools are essential for writing, managing, and executing code.

Follow the instructions below to download and install the following tools on your computer. Choose the instructions that match your operating system (Windows, Mac, or Linux/Ubuntu).

### VSCode

A programming editor.

+ All Platforms: [code.visualstudio.com/download](code.visualstudio.com/download)
  + **Windows**:  
    Download the installer from [https://code.visualstudio.com/](https://code.visualstudio.com/) and run the `.exe` file.

  + **Mac**:  
    Download the installer from [https://code.visualstudio.com/](https://code.visualstudio.com/) and open the `.zip` file. Drag the app to your Applications folder.

  + **Linux (Ubuntu)**:  
    Open a terminal and run:

    ```sh
    sudo apt update
    sudo apt install code
    ```

    Or download the `.deb` package from the website and install it.

+ YouTube Tutorial video: [VS Code Team Tutorial](https://www.youtube.com/watch?v=B-s71n0dHUk)

### Git Setup

Allows you to transfer files to and from a GitHub repository, in addition to adding version control to projects.

#### Download and Install Git

+ [https://github.com/git-guides/install-git](https://github.com/git-guides/install-git)

#### Create Your Free Account

+ Sign up: [github.com/signup](https://github.com/signup)
+ **Essential for:**
  + Accessing class repositories
  + Submitting your work for grading
  + Version control

#### Set Up Your GitHub Profile

Complete your profile for better collaboration.

1. **Add a profile picture**
 - Click on your avatar in the top-right corner
 - Select "Settings"
 - Upload a clear photo of yourself

1. **Add your name and bio**
 - Go to "Public profile" section
 - Add your full name (first and last)
 - Write a brief bio (e.g., "Computer Science student at Allegheny College")

1. **Add your location and email**
 - Location: "Meadville, PA" (or your hometown)
 - Email: Use your preferred contact email

1. **Set up your README**
 - Consider creating a profile README to showcase your work
 - Optional but recommended for building your professional presence

#### Set up your SSH Keys for use with GitHub

SSH keys provide secure authentication for Git operations and server access. **Use VS Code's integrated terminal for all these commands.**

#### Generate the SSH Key Pair

1. **Open VS Code's integrated terminal**
2. **Run the SSH key generation command:**

```bash
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

   + Press Enter to accept the default file location
   + Enter a passphrase when prompted (you will need to enter it each time you send your work to GitHub, press Enter twice if you don't want to create passphrase)

#### Add the Public Key to GitHub

1. **Copy your public key from VS Code's terminal:**

  ```bash
  cat ~/.ssh/id_rsa.pub
  ```

2. **Add to GitHub:**

   + Go to GitHub Settings → SSH and GPG keys
   + Click "New SSH key"
   + Paste your public key
   + Give it a descriptive title (e.g., "Mac Machine")

3. **Test the connection from VS Code's terminal:**

  ```bash
   ssh -T git@github.com
   ```

  *  You should see a message similar to: "You've successfully authenticated..."

### Python3: A programming language

+ **Windows**:  
  Download the installer from [https://www.python.org/downloads/windows/](https://www.python.org/downloads/windows/) and run the `.exe` file.

+ **Mac**:

  Python is often pre-installed on MacOS, but it may be an older version which might need updating. I have found in some cases that by simply typing `python3` in the terminal, MacOS may automatically ask the user whether it can automatically install updates from `XCode`. Follow the prompts to complete the installation.

  Install using Homebrew which is available from [https://brew.sh/](https://brew.sh/). Open a terminal and run:
  
  ```sh
  brew install python
  ```

  Or download from [https://www.python.org/downloads/mac-osx/](https://www.python.org/downloads/mac-osx/).

+ **Linux (Ubuntu)**:

  Python is often pre-installed on Ubuntu, but if you need to install or upgrade it.

  Open a terminal and run:

  ```sh
  sudo apt update
  sudo apt install python3
  ```

### GatorGrade

This activity will be checked by Gatorgrade for completion when it is submitted to your GitHub repository. You can also check your work locally if you want before you submit it. To do so, you will first need to install the `GatorGrade` checking python code before it can be run. If you already have `GatorGrad` installed, then, there is need to reinstall it. 

 + You will used `pipx` to install `GatorGrade`. If you do not have `pipx` already installed, then please follow the instructions at [https://pipx.pypa.io/stable/installation/](https://pipx.pypa.io/stable/installation/) to install it on your local machine.
 + Install `Gatorgrade` by running the following command in your terminal or command prompt:

  ```bash
  pipx install gatorgrade
  ```

### Checking Your Work

 + Navigate to the root directory of this project in your terminal or command prompt to run the following command. Note, you must be inside the project directory for the below command to work to check your work.

  ```bash
  gatorgrade --config config/gatorgrade.yml
  ```

---

## Part 2: Maze Solving and Instruction Exchange

**Partner work**: Work with one partner.

**Deliverable**: A written set of instructions and a critique of the instructions you received from your partner.

**Instructions**: Computer code is simply a listing of instructions that provide a computer with the steps needed to complete a task. Interestingly, the task of writing code is very similar to the task of writing instructions for a person to follow.

Writing clear and precise instructions is a crucial skill in programming and collaboration. In this part of the project, you will practice this skill by solving a maze and then exchanging your solution steps with your partner. Remember that when you are working with a list of instructions prepared by someone else, you must follow them exactly as given, without making assumptions or adding your own interpretations.

1. Pair up with a partner. Each person selects a maze diagram to solve.
2. Each person works independently to solve their chosen maze.
3. As you solve the maze, write down the *exact* steps and any important information needed to reach the solution.
4. Exchange your maze and instructions with your partner.
5. Each person must follow only the instructions provided by their partner to attempt solving the new maze.
6. After completing the maze, write a critique (see `writing/reflection.md`) of the instructions you received. Note what worked well and what could be improved.
7. Each member of the course is to submit their own copy of the work via their personal GitHub repository. Please be sure to include the name of your partner in your submission. Please also submit your work with a minimum of five (5) commits to your repository. (Note: These five commits are to encourage good habits when using `Git` and `GitHub`.)

## Reflection Questions

Please open the `writing/reflection.md` file and answer the questions there. Be sure to replace all instances of `To-Do` with your answers. If you have any questions about the reflection, please ask!
