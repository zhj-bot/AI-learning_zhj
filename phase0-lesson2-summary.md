# Phase 0 Lesson 2 Summary: Git & Collaboration

## What This Lesson Was About

This lesson introduced Git as a way to save learning progress, experiment
safely, and sync work to GitHub.

Git can be understood as a project time machine. It records snapshots of files
so you can see what changed, go back to earlier versions, and continue work on
another computer.

## Key Concepts

### Working Directory

The working directory is the folder where files are edited.

In this repository, the working directory is:

```powershell
C:\Users\lenovo\Documents\AI学习
```

### Staging Area

The staging area is where Git stores the changes selected for the next commit.

Important idea:

```text
git add = choose which changes will be saved in the next snapshot
```

### Commit

A commit is a saved snapshot in Git history.

Important idea:

```text
git commit = save the selected changes as a snapshot
```

The commit message explains what changed.

### Branch

A branch is a separate line of work.

Branches are useful because they let you experiment without damaging the main
line of work.

Example from this lesson:

```text
master/main: original learning notes
my-progress: branch used for practice changes
```

### Merge

Merge combines changes from one branch into the current branch.

Example:

```powershell
git merge my-progress
```

This means:

```text
Bring the changes from my-progress into the branch I am currently on.
```

### Remote Repository

A remote repository is a copy of the local Git repository on a service such as
GitHub.

Important idea:

```text
commit saves locally
push uploads to GitHub
```

## Commands Practiced

```powershell
git status
git add phase0-lesson2-git.md
git commit -m "Add Git lesson notes"
git branch my-progress
git switch my-progress
git log --oneline --decorate
git switch master
git merge my-progress
git branch -M main
git remote add origin https://github.com/zhj-bot/AI-learning_zhj.git
git push -u origin main
```

## Exercise Answers and Feedback

### Question 1

What does `git add` do?

Your answer:

```text
git add points to which files changed
```

Feedback:

The idea was close, but the more accurate meaning is:

```text
git add selects file changes and puts them into the staging area for the next
commit.
```

### Question 2

What does `git commit` do?

Your answer:

```text
git commit explains this change
```

Feedback:

The commit message explains the change, but the commit itself does more:

```text
git commit saves the staged changes as a snapshot in Git history.
```

### Question 3

What problem does a branch solve?

Your answer:

```text
branch solves the problem of not being able to return after changes, or
damaging the main line.
```

Feedback:

Correct. A branch creates a safe experiment line so changes can be tested before
being merged into the main branch.

### Question 4

What does `git merge my-progress` do?

Your answer:

```text
It merges my-progress into the current branch.
```

Feedback:

Correct.

## Learning Progress

Current status:

```text
Phase 0 Lesson 2: completed
```

You understand the main Git workflow:

- Check changes with `git status`.
- Stage changes with `git add`.
- Save snapshots with `git commit`.
- Use branches for safe experiments.
- Merge a branch back into the current branch.
- Push local commits to GitHub.

Needs review:

- Difference between `git add` and `git commit`.
- Difference between local commit and GitHub push.

Next recommended lesson:

```text
Phase 0 Lesson 3
```
