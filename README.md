# Chicago Lakefront Conservation

This repository contains code and analysis for the Chicago Lakefront Conservation research project.

## Getting Started

### 1. Clone the Repository

If you have not downloaded the project yet:

```bash
git clone https://github.com/arinazhou/chicago-lakefront-conservation.git
cd chicago-lakefront-conservation
```

### 2. Create Your Own Branch

Each person should work on their own branch instead of making changes directly on `main`.

First, make sure you have the newest version of `main`:

```bash
git switch main
git pull origin main
```

Then create your own branch:

```bash
git switch -c your-name
```

For example:

```bash
git switch -c arina
```

You only need to create your branch once.

After that, you can switch to it anytime with:

```bash
git switch arina
```

To check which branch you are currently using:

```bash
git branch
```

The branch with `*` next to it is your current branch.

---

## Working on the Project

Before starting work, make sure you are on your own branch:

```bash
git switch your-name
```

Then check your repository:

```bash
git status
```

Make your changes normally: edit code, add notebooks, update documentation, etc.

---

## Saving Your Changes

After you finish some work, check what changed:

```bash
git status
```

Add your changes:

```bash
git add .
```

Commit them:

```bash
git commit -m "Describe what you changed"
```

For example:

```bash
git commit -m "Add nighttime light preprocessing"
```

Then push your branch to GitHub:

```bash
git push
```

The first time you push a new branch, Git may ask you to set the upstream branch. Run:

```bash
git push -u origin your-name
```

For example:

```bash
git push -u origin arina
```

After doing this once, future pushes only require:

```bash
git push
```

---

## Typical Workflow

Most of the time, your workflow will simply be:

```bash
# Make sure you are on your branch
git switch your-name

# Check your changes
git status

# Stage your changes
git add .

# Commit
git commit -m "Describe what you changed"

# Push to GitHub
git push
```

For example:

```bash
git switch arina

git status
git add .
git commit -m "Add light color analysis"
git push
```

---

## Getting Updates From `main`

If other people's work has been merged into `main`, update your local `main`:

```bash
git switch main
git pull origin main
```

Then return to your branch:

```bash
git switch your-name
```

Merge the newest `main` into your branch:

```bash
git merge main
```

Now your branch contains the latest shared changes.

---

## Merging Your Work Into `main`

Do **not** directly push your experimental work to `main`.

Instead:

1. Push your personal branch to GitHub.
2. Open the repository on GitHub.
3. Create a **Pull Request** from your branch into `main`.
4. Review the changes.
5. Merge the Pull Request after the changes are ready.

The basic workflow is:

```text
main
  │
  ├── arina
  │     └── work → commit → push → Pull Request
  │
  ├── person-2
  │     └── work → commit → push → Pull Reques
```
