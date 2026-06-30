# Submission Recipe

**CSCI 101 – how to submit every stage of the writing project**

Every stage of the Ethics in Technology project is submitted the same way: as a Pull Request **inside your own repository**. Once you have done it once (see *PR 00* below), every stage is the same seven steps — only the stage number changes. Bookmark this page.

<div class="step">

**Which guide do I use?** Three short docs, in order:

- [GitHub Setup Guide](github-setup-guide.md) (Session 1) — install and configure Git, once.
- [Git Setup Tutorial](GIT-SETUP-TUTORIAL.md) (Session 2) — the detailed PR 00 walkthrough, your first time through.
- **This Submission Recipe** — your quick reference for every stage after that.

</div>

<div class="success">

**You are not graded on Git mechanics.** Every stage's points are for the **content** of your work. If a submission has a mechanical problem — wrong branch name, missing folder, forgotten PR — you'll be asked to fix it, and it will **not** cost you content points. Getting the mechanics right is required to submit; it is not part of your grade.

</div>

## One-time setup (Week 1)

<div class="step">

1.  Set up Git and GitHub (see the [GitHub Setup Guide](github-setup-guide.md)). You're ready when `git --version`, `git config user.name`, and `git config user.email` all return values.
2.  Create your own project repository from the course template: on **CSCI101_F26Project**, click **"Use this template" → "Create a new repository."** Name it `csci101-project-firstname-lastname`.
3.  **Add your instructor as a collaborator** so they can review your work: your repo → Settings → Collaborators → add the instructor's GitHub username, **@INSTRUCTOR-HANDLE** (your instructor will confirm this in class / on Canvas). **Important:** the invite expires after 7 days, and your instructor cannot see or grade your work until it's accepted — so send it in Week 1 and let them know.
4.  Clone your repo to your computer: `git clone <your-repo-URL>`

</div>

## PR 00: the practice run (do this once, no points)

<div class="step">

Before your first real stage, rehearse the whole loop with throwaway content so the first *graded* submission is never your first-ever Pull Request.

1.  Branch: `git checkout -b pr00`
2.  Create a folder `pr00/` and add a file `hello.md` that says: "Hi, I'm \[your name\], practicing the workflow."
3.  `git add pr00 && git commit -m "PR 00 - practice - FirstName LastName"`
4.  `git push -u origin pr00`
5.  On GitHub, open a Pull Request: base `main`, compare `pr00`.
6.  Confirm the submission-check comment appears, then merge your own PR.

**You're ready** when PR 00 is opened and merged. That proves your whole pipeline works.

</div>

## The Recipe (every stage, 1–6)

Replace `#` with the stage number. That's the only thing that changes.

<div class="step">

1.  **Sync:** `git checkout main && git pull`
2.  **Branch:** `git checkout -b stage#`
3.  **Folder:** create `stage#/` and add your deliverable file(s) — the stage page tells you which
4.  **Commit:** `git add stage# && git commit -m "Stage # - FirstName LastName"`
5.  **Push:** `git push -u origin stage#`
6.  **Open a Pull Request** on GitHub: base `main`, compare `stage#`
7.  **Check the submission-check comment** is all green, then leave the PR open for your instructor to review (they will comment and merge it)

</div>

<div class="success">

**What counts as "submitted":** opening the Pull Request by the deadline. You do **not** merge your own stage PRs — leave them open; your instructor reviews and merges them. (The one exception is the no-points **PR 00** practice run, which you merge yourself.)

</div>

<div class="step">

### Updating a submission

Made changes after opening the PR? Just commit and push to the same branch — the PR updates automatically:

    git add stage#
    git commit -m "Update Stage # - description"
    git push

</div>

<div class="step">

### Stage → Pull Request

Each stage is one Pull Request in your own repo. The numbers line up directly:

| Stage    | Branch / folder | Pull Request      |
|----------|-----------------|-------------------|
| Practice | `pr00`          | PR 00 (no points) |
| Stage 1  | `stage1`        | PR 1              |
| Stage 2  | `stage2`        | PR 2              |
| Stage 3  | `stage3`        | PR 3              |
| Stage 4  | `stage4`        | PR 4              |
| Stage 5  | `stage5`        | PR 5              |
| Stage 6  | `stage6`        | PR 6              |

Stage to Pull Request

</div>

<div class="warning">

### Stuck on the mechanics?

That's fine and it won't cost you points. Post in the discussion board or bring it to office hours. The mechanics are a skill you're *practicing*, not a test.

</div>

------------------------------------------------------------------------

*CSCI 101 – Submission Recipe*
