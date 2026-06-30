# GitHub Tutorial: Your First Pull Request (PR 00)

## CSCI 101 - Session 2 of 2

---

## Prerequisites

**Before starting this tutorial, complete Session 1 (github-setup-guide.html):**
- GitHub account created
- Git installed on your computer
- Git configured with your name and email

**Time needed**: 20-30 minutes

---

## What We'll Accomplish

By the end of this tutorial you will have:
- Created **your own** project repository from the course template
- Added your instructor as a collaborator
- Cloned it to your computer
- Completed **PR 00**, a zero-stakes practice Pull Request

PR 00 rehearses the exact workflow you'll use for all six project stages, so
your first *graded* submission is never your first-ever Pull Request. There is
**no fork and no `upstream` remote** — you work entirely inside your own repo.

> **You are not graded on Git mechanics.** PR 00 carries no points. Its only
> purpose is to make sure your pipeline works.

---

## Part 1: Create Your Project Repository

1. Go to the course project template: **`CSCI101_F26Project`** (your
   instructor will give you the link).
2. Click the green **"Use this template"** button, then **"Create a new
   repository."**
3. Name it `csci101-project-firstname-lastname` (use your own name).
4. Keep it **Private**, then click **"Create repository."**

You now have your OWN copy of the project repository.

---

## Part 2: Add Your Instructor as a Collaborator

So your instructor can read and review your Pull Requests:

1. In your new repo, go to **Settings → Collaborators**.
2. Click **"Add people"** and enter your instructor's GitHub username:
   **@INSTRUCTOR-HANDLE** (your instructor will confirm this in class / on Canvas).
3. Your instructor will accept the invitation.

**Important:** the invitation **expires after 7 days**, and your instructor
**cannot see or grade your work** until it's accepted. Send it in Week 1 and let
your instructor know. This is the same way developers share a repository in the
real world.

---

## Part 3: Clone to Your Computer

### Step 3.1: Get Your Repo's URL
1. On your repo, click the green **"Code"** button.
2. Copy the URL (HTTPS is fine).

### Step 3.2: Clone It
```bash
# Move to where you keep your coursework, e.g.:
cd ~/Documents        # Mac
cd /c/Users/YourName/Documents   # Windows

# Clone YOUR repository
git clone <your-repo-URL>
cd csci101-project-firstname-lastname
```

### Step 3.3: Verify You're in the Right Place
```bash
ls
```
You should see the project files, including `README.md`,
`SUBMISSION-RECIPE.md`, and `Ethics_in_Technology.md`.

---

## Part 4: Create PR 00 (Your First Pull Request)

### Step 4.1: Create a Branch
```bash
git checkout -b pr00
```

### Step 4.2: Create a Folder and a File
```bash
mkdir pr00
```
Create a file `pr00/hello.md` with this content (use your own name):
```markdown
# Hello

Hi, I'm John Smith, practicing the workflow.
```

### Step 4.3: Add and Commit
```bash
git add pr00
git commit -m "PR 00 - practice - John Smith"
```

### Step 4.4: Push
```bash
git push -u origin pr00
```

If prompted for a password, use a **Personal Access Token**, not your account
password (GitHub → Settings → Developer settings → Personal access tokens →
generate one with the `repo` scope).

---

## Part 5: Open the Pull Request

1. Go to your repo on GitHub. You'll see a banner: **"pr00 had recent
   pushes."** Click **"Compare & pull request."**
2. Confirm the settings:
   - Base: `main`
   - Compare: `pr00`
   (Both are in **your own** repo — there is no other repository involved.)
3. Title it `PR 00 - practice - John Smith` and click **"Create pull
   request."**

### The submission check
Within a minute, a friendly **submission-check** comment appears on your PR
confirming your branch and folder names. It is advisory only and never blocks
your work. When it's green, **merge your own PR** (the "Merge pull request"
button).

**You're ready** once PR 00 is opened and merged. Your whole pipeline works.

---

## Congratulations!

You've completed a Pull Request using the same workflow professional developers
use worldwide, entirely in your own repository.

**From here, every project stage is the same seven steps** — only the stage
number changes (Stage 1 = PR 1, … Stage 6 = PR 6). See **SUBMISSION-RECIPE.md**
for the full reference.

> **One difference for graded stages:** you merged PR 00 yourself because it's
> just practice. For the six graded stages, **open the Pull Request and leave it
> open** — your instructor reviews it and merges it. Opening the PR by the
> deadline is what counts as submitted.

---

## Quick Reference Card

```bash
# For each stage (# = stage number 1-6)
git checkout main
git pull
git checkout -b stage#
# put your files in a stage# folder, then:
git add stage#
git commit -m "Stage # - FirstName LastName"
git push -u origin stage#
# On GitHub: open a Pull Request (base: main, compare: stage#)
```

---

## Troubleshooting

### "Permission denied" when pushing
- **Cause**: You may be pushing to a repo that isn't yours.
- **Fix**: Confirm `git remote -v` shows YOUR repository.

### "Fatal: not a git repository"
- **Cause**: You're not in the right folder.
- **Fix**: `cd` into your project folder.

### Can't find Git Bash (Windows)
- **Fix**: Search "Git Bash" in the Start Menu.

### Password authentication was removed
- **Fix**: Use a Personal Access Token instead of your password
  (GitHub → Settings → Developer settings → Personal access tokens).

---

*Questions? Check SUBMISSION-RECIPE.md or ask during office hours!*
