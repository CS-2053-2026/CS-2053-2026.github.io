# Using Git for Labs and Assignments

We will be using [Git](https://git-scm.com/) for accessing example code and submitting assignments. Git is a very powerful tool, but the way we will use it for the course will be quite simple. In all cases, repositories will be created for you and you will "clone" the repositories to get started. Git is installed on the lab computers, but will need to ne installed if using your own.

We ask that you follow these below carefully, and only stray from them if you know what you are doing. There are lots of great git learning resources online, like the free [Pro Git Book](https://git-scm.com/book/en/v2).

Before you get started with the details in this page you should complete the steps in [Software Setup and Requirements page](pages/cs2053-requirements-and-setup.md).

## Your GitHub Account

You are required to have a GitHub account for this course.

You can create a [new Github account here](https://github.com/signup) or use an existing Github account.

When using Git we ask that you follow these instructions below carefully, and only stray from them if you know what you are doing.

## Accessing Repos for the Class Activities

Each of the class's activities and projects will be hosted on GitHub, and you will be provided with an invite link via D2L to each as they become available.

After accepting the invite to the repo in question, a fork (new copy) of that repo will be made for you to use.
For example, accepting `https://github.com/CS-2053-2026/Project_1` a new repo called `https://github.com/CS-3035-2024/Project_1-YourUserName` will be created for you.

Only you, the instructors, and TAs will have access to your repos.

### Accessing and Modfying those Repos with Git

There are many ways to interact with Git, but for the purposes of this course, we recomend one of 2 options:

1.  **CLI** - You can interact with git directly through your terminal. See the basics [here](https://git-scm.com/cheat-sheet).
2.  **Github Desktop** - GitHub provides an easy [GUI interface](https://desktop.github.com/download/) (for mac and windows) which works as well.

## Submitting Your Work – _Committing_ and _Pushing_ Your Code

GitHub gives you a lot of flexibility in how you manage your work.  
For this course, we will use it in a **very simple and consistent way**:

- You **commit** your changes locally
- You **push** those commits to GitHub

  **Both steps are required.**  
  If you commit but do not push, your work stays on your computer and **will not be visible to the instructors**.

### Committing

Committing takes the changes you have made and **records a snapshot** of them in your local repository.  
Think of a commit as a save point with a message explaining what changed.

#### CLI

1. Open a terminal in your project directory.
2. Check which files have changed:

```bash
git status
```

3. Stage your changes:

```bash
git add .
```

> This stages **all** changed files. You can also stage individual files if needed.

4. Commit your changes with a short, clear message:

```bash
git commit -m "Brief description of your changes"
```

You can commit as often as you like.  
Commits are **local only** until you push them to GitHub.

#### GH Desktop

1. Make sure you have the correct repository selected under **Current Repository**.
2. Confirm that all the changes you want to submit appear under **Changes**.
3. Enter a short summary describing what you changed.
4. Click **Commit to main** (or the current branch).

> Commit early, commit often. This creates a clear history and protects you from losing work.

### Pushing Your Code

Pushing uploads your local commits to GitHub so they are backed up and available for grading.

For assignments and lab exams, **only the most recent version pushed to GitHub before the deadline will be graded** (unless otherwise specified).

#### CLI

After committing:

```bash
git push
```

If this is your first push, you may be prompted to authenticate with GitHub.
This means you will need to set your email and username for verification. You only need to do so once on any machine you use, and you can do so via these commands:

- `git config --global user.email *your@githubemailaddress.com*`
- `git config --global user.name *yourGithubUsername*`

#### GH Desktop

1. Make sure all your work is committed.
2. Click **Push origin** at the top of the window.
3. Wait for the push to complete.

**Always double-check** by visiting the GitHub website and confirming that your latest commit appears there.

### Pulling Changes

Pulling retrieves changes from GitHub and merges them into your local repository.  
You may need this when:

- Working on multiple computers
- Collaborating with others
- An instructor has pushed additional code or fixes

#### CLI

```bash
git pull
```

If you have uncommitted changes, Git may refuse to pull. Commit first.

#### GH Desktop

1. Open the correct repository.
2. Click **Fetch origin**.
3. If updates are available, click **Pull origin**.

### Final Checklist Before Submission

Before the deadline, make sure:

- ✅ You committed your changes
- ✅ You pushed your commits to GitHub
- ✅ You can see your latest commit on the GitHub website

If it’s not on GitHub, **it doesn’t exist for grading**.
