# Mars Rover Autonomous Subsystem Induction – Submission Instructions

Welcome! Please follow these detailed steps to submit your ROS2 induction package to this repository. 
---

## Table of Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Step 1: Clone the Repository](#step-1-clone-the-repository)
- [Step 2: Create the `src/` Directory (If Needed)](#step-2-create-the-src-directory-if-needed)
- [Step 3: Create Your Branch](#step-3-create-your-branch)
- [Step 4: Copy Your ROS2 Package](#step-4-copy-your-ros2-package)
- [Step 5: Add, Commit, and Push Your Changes](#step-5-add-commit-and-push-your-changes)
- [Step 6: Add Documentation and Video Link](#step-6-add-documentation-and-video-link)
- [Checklist Before Submission](#checklist-before-submission)
- [Need Help?](#need-help)

---

## Overview

You are required to:

- Create your own branch in this repository.
- Add your ROS2 package inside a `src/` directory.
- Document your package and submit a demonstration video link.
- Commit and push your changes for review.

---

## Prerequisites

- A GitHub account with push access to this repository (contact a mentor if you need access).
- Git installed on your computer.
- Your ROS2 package ready in your local ROS2 workspace (typically `~/ros2_ws/src/<your_package_folder>`).

---

## Step 1: Clone the Repository

Open your terminal and run:
```
git clone https://github.com/jarjlol/Project-Kratos-Autonomous-Induction.git
cd Project-Kratos-Autonomous-Induction
```
---

## Step 2: Create the `src/` Directory (If Needed)

Check if a `src/` directory exists:
```
ls
```

If you **do not** see a `src/` folder, create one:

```
mkdir src
```

---

## Step 3: Create Your Branch
**If you are uploading your first induction task, you need to create your own branch, which you will use throughout the induction process.**

Replace `<yourname>` with your name:

```
git checkout -b induction-<yourname>
```

Push your branch to GitHub:

```
git push -u origin induction-<yourname>
```

---

## Step 4: Copy Your ROS2 Package

Assuming your package is in `~/ros2_ws/src/<your_package_folder>`, copy it into the repo’s `src/` folder:

```
cp -r ~/ros2_ws/src/<your_package_folder> ./src/
```

---

## Step 5: Add, Commit, and Push Your Changes

Add your package to version control (refer Need Help section in case of error):

```
git add src/<your_package_folder>
git commit -m "Add ROS2 induction package for <yourname>"
git push
```

---

## Step 6: Add Documentation and Video Link

1. **Inside your package folder (`src/<your_package_folder>`), create or update a `README.md` file.**
   - Briefly describe what your package does.
   - Give clear instructions on how to build and run your package.
   - List any dependencies.
   - **Include a link to your demonstration video** (upload your video to Google Drive, Dropbox, etc., and paste the share link in the README).

   

---

## Checklist Before Submission

- [ ] Created a branch named `induction-<yourname>`
- [ ] Added your ROS2 package to `src/`
- [ ] Included a `README.md` in your package folder with instructions and video link
- [ ] Committed and pushed all changes

---

## Need Help?

- If you encounter issues with GitHub authentication, ensure you are using a [Personal Access Token (PAT)](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) instead of your password.
- For Git or ROS2 questions, ask in the team’s communication channel or contact a mentor.
- Refer to the [GitHub Docs](https://docs.github.com/) for more help.

---

**Good luck! We look forward to seeing your work.**
