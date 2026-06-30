# GitHub Setup Guide

**CSCI 101 – Session 1 of 2**

<span class="time-estimate">Estimated time: 20-30 minutes</span>

Complete this guide **before** accessing the GitHub tutorial. By the end, you'll have:

- A GitHub account
- Git installed on your computer
- Git configured with your identity
- An understanding of README.md files

------------------------------------------------------------------------

## Part 1: Create Your GitHub Account

<span class="time-estimate">5-10 minutes</span>

<div class="step">

### Step 1.1: Sign Up

1.  Go to <a href="https://github.com" target="_blank" rel="noopener noreferrer">https://github.com</a>
2.  Click the **"Sign up"** button
3.  Choose a username (this will be visible to employers!)

**Username tips:**

- <span class="good">✓ Good:</span> `john-smith`, `jsmith2025`, `johnsmith`
- <span class="bad">✗ Avoid:</span> `coolgamer123`, `dragonslayer99`

</div>

<div class="step">

### Step 1.2: Verify Your Email

1.  Check your email inbox
2.  Click the verification link from GitHub

</div>

<div class="step">

### Step 1.3: Complete Your Profile

1.  Click your avatar (top-right corner) → **"Your profile"**
2.  Click **"Edit profile"**
3.  Add:
    - Your real name
    - A brief bio: "Computer Science student at \[University\]"
    - Your location (optional)

</div>

------------------------------------------------------------------------

## Part 2: Install Git

<span class="time-estimate">5-10 minutes</span>

### For Windows Users

<div class="step">

1.  Go to <a href="https://git-scm.com/download/windows" target="_blank" rel="noopener noreferrer">https://git-scm.com/download/windows</a>
2.  Download the installer
3.  Run the installer
4.  Use these settings when prompted:
    - **Default editor:** Choose "Use Notepad as Git's default editor"
    - **PATH environment:** Choose "Git from the command line and also from 3rd-party software"
    - **Line endings:** Choose "Checkout Windows-style, commit Unix-style"
5.  Click "Next" for all other screens

</div>

### For Mac Users

<div class="step">

1.  Open **Terminal** (find it in Applications → Utilities)
2.  Type: `git --version`
3.  If you see a version number, Git is already installed! Skip to Part 3.
4.  If prompted to install, click **"Install"**
5.  If nothing happens, download from <a href="https://git-scm.com/download/mac" target="_blank" rel="noopener noreferrer">git-scm.com/download/mac</a>

</div>

### For Linux Users

<div class="step">

Open a terminal and run:

    # Ubuntu/Debian:
    sudo apt update && sudo apt install git

    # Fedora:
    sudo dnf install git

</div>

### Verify Installation

<div class="step">

1.  **Windows:** Open "Git Bash" (search in Start Menu)
2.  **Mac/Linux:** Open Terminal
3.  Type: `git --version`
4.  You should see something like: `git version 2.42.0`

</div>

<div class="success">

**Success!** If you see a version number, Git is installed correctly.

</div>

------------------------------------------------------------------------

## Part 3: Configure Git

<span class="time-estimate">2-3 minutes</span>

<div class="step">

### Step 3.1: Open Your Terminal

- **Windows:** Open "Git Bash"
- **Mac/Linux:** Open Terminal

</div>

<div class="step">

### Step 3.2: Set Your Identity

Replace the name and email with YOUR information:

    git config --global user.name "Your Full Name"
    git config --global user.email "your.email@example.com"

**Example:**

    git config --global user.name "John Smith"
    git config --global user.email "jsmith@university.edu"

</div>

<div class="step">

### Step 3.3: Verify Configuration

    git config --list

You should see your name and email in the output.

</div>

------------------------------------------------------------------------

## Part 4: Understanding README.md Files

<span class="time-estimate">5 minutes (reading)</span>

Before you start using GitHub, it's important to understand one of its most important features: the **README.md** file.

### What is a README.md?

A **README.md** file is the "front page" of any repository. When you visit a repository on GitHub, the README.md content is automatically displayed below the file listing.

- **README** = "Read me first!" - essential information about the project
- **.md** = Markdown format (a simple way to format text)

### Why README.md Matters

Every professional repository has a README.md because it:

1.  **Explains the project** - What is this? What does it do?
2.  **Provides instructions** - How do I use it?
3.  **Makes a first impression** - Employers and collaborators see this first
4.  **Documents your work** - Future you will thank present you!

### What Goes in a README.md?

A good README typically includes:

- **Title** - Name of the project
- **Description** - What it is and why it exists
- **Contents** - What files are included
- **Author** - Who created it

### Markdown Basics

README files use **Markdown** syntax for formatting:

| What you type        | What you get    |
|----------------------|-----------------|
| `# Heading`          | Large heading   |
| `## Smaller Heading` | Smaller heading |
| `**bold text**`      | **bold text**   |
| `*italic text*`      | *italic text*   |
| `- item`             | Bullet point    |

Markdown Basics Reference

You'll create README.md files for each of your submissions in the GitHub tutorial!

------------------------------------------------------------------------

## Setup Complete!

<div class="success">

### Checklist - Before Moving On:

- I have a GitHub account with my real name
- Git is installed on my computer
- Git is configured with my name and email
- I understand what a README.md file is for

</div>

### Next Steps

You're now ready for **Session 2: The GitHub Tutorial**

Go to the course repository to continue:

    https://github.com/csci101/csci101

Start with the **GIT-SETUP-TUTORIAL.md** file.

------------------------------------------------------------------------

## Troubleshooting

### "git" is not recognized (Windows)

<div class="warning">

**Solution:** Make sure you're using "Git Bash", not Command Prompt or PowerShell.

</div>

### "Please tell me who you are" error

<div class="warning">

**Solution:** Run the git config commands from Part 3 again.

</div>

### Can't find Terminal (Mac)

<div class="warning">

**Solution:** Press Cmd+Space, type "Terminal", and press Enter.

</div>

------------------------------------------------------------------------

*CSCI 101 – GitHub Setup Guide*
