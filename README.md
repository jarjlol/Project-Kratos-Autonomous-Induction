# Induction Submission Instructions

Welcome! Follow these steps to submit your ROS2 induction package as a private submodule.

---

## Table of Contents

- [Step 1: Create Your Private Repository](#step-1-create-your-private-repository)
- [Step 2: Add the Admin as a Collaborator](#step-2-add-the-admin-as-a-collaborator)
- [Step 3: Add Your ROS2 Package to Your Repo](#step-3-add-your-ros2-package-to-your-repo)
- [Step 4: Add Your Repo as a Submodule to the Main Induction Repo](#step-4-add-your-repo-as-a-submodule-to-the-main-induction-repo)
- [Notes & Best Practices](#notes--best-practices)
- [Troubleshooting](#troubleshooting)

---

## Step 1: Create Your Private Repository

1. Go to [GitHub](https://github.com/) and create a **new private repository**.  
   Suggested name: `induction-<your name>`
2. Do **not** initialize with a README, .gitignore, or license (keep it empty).

---

## Step 2: Add the Admin as a Collaborator

1. Go to your new private repository on GitHub.
2. Click on **Settings**.
3. In the left sidebar, click **Collaborators & teams** or **Manage access**.
4. Click **Add people**.
5. Enter the admin’s GitHub username: `jarjlol`, `Vishesh-Ag-BITSG`
6. Click **Add** or **Invite**.
7. Wait for the admin to accept the invitation before proceeding.

---

## Step 3: Add Your ROS2 Package to Your Repo

1. Clone your private repository to your computer:
   ```
   git clone https://github.com//induction-<your name>.git
   cd induction-<your name>
   ```
2. Copy your ROS2 package files into this directory.
3. Add, commit, and push your code:
   ```
   git add .
   git commit -m "Initial commit: Add my ROS2 induction package"
   git push
   ```

---

## Step 4: Add Your Repo as a Submodule to the Main Induction Repo

1. Clone the main induction repository:
   ```
   git clone https://github.com/jarjlol/Project-Kratos-Autonomous-Induction.git
   cd Project-Kratos-Autonomous-Induction
   ```
2. Make sure you’re on your own branch (use the same branch throughout the induction. Make sure you type this branch name correctly):
   ```
   git checkout -b induction-<your name>
   ```
3. Create the `src/` directory if it doesn't exist:
   ```
   mkdir -p src
   ```
4. Add your repository as a submodule inside the `src/` directory:
   ```
   git submodule add https://github.com/<your GitHub username>/induction-<your name>.git src/induction-<your name>
   ```
5. Stage and commit the submodule addition:
   ```
   git add .gitmodules src/induction-<your name>
   git commit -m "Add my induction package as a submodule"
   git push --set-upstream origin induction-<your name>
   ```

---

## Notes & Best Practices

- **Keep your induction package repository private** and only invite the admin and yourself as collaborators.
- To update your package, push changes to your own repo, then update the submodule pointer in the main repo and commit again.

---

## Troubleshooting

- If you see an error about the submodule path already existing, make sure you are not duplicating submodule names.
- If you forget to initialize submodules after cloning the main repo, run:
  ```
  git submodule update --init --recursive
  ```
- If you encounter issues with GitHub authentication, ensure you are using a [Personal Access Token (PAT)](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) instead of your password.
---

**Thank you! Wishing you the best of luck!**
