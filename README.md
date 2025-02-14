# Contributing to this Project

This document outlines the steps to contribute to this project using forks and pull requests.


## 1. Fork the Repository

On the GitHub page for the project, click the "Fork" button in the upper-right corner. This creates a copy of the repository in your GitHub account.



## 2. Clone Your Fork

Clone your forked repository to your local machine using Git:

(Replace `your-username` with your GitHub username and `repository-name` with the name of the repository.)

git clone https://github.com/your-username/repository-name.git

cd repository-name



## 3. Add the Upstream Remote

Add the original repository as an "upstream" remote to keep your local copy in sync:

git remote add upstream https://github.com/original-owner/repository-name.git

(Replace `original-owner` with the original owner's GitHub username and `repository-name` with the name of the repository.)



## 4. TO CONTRIBUTE : Create a Feature Branch

Before starting work on a new feature or bug fix, create a new branch:

git checkout -b feature/feature-branch-name

Always prefix 'feature/' followed by a descriptive name of your feature branch (`feature-branch-name`)



## 5. Make Changes and Commit

Make your changes to the code and commit them with clear, descriptive commit messages:

git add .

git commit -m "Add a descriptive commit message"



## 6. Push to Your Fork

Push your feature branch to your forked repository on GitHub:

git push origin feature/feature-branch-name



## 7. Keep Your Fork Updated

Before creating a pull request, ensure your fork is up-to-date with the upstream repository:

git fetch upstream

git checkout main

git merge upstream/main # or git rebase upstream/main

git push origin main

Resolve any conflicts that may arise during the merge.



## 8. Create a Pull Request

On GitHub, navigate to your forked repository. You should see a banner prompting you to create a pull request for your newly pushed branch. Alternatively, you can go to the "Pull requests" tab and click "New pull request".

Select your feature branch as the "compare branch" and the upstream repository's `main` (or `develop`) branch as the "base branch".

Provide a clear title and description for your pull request.



## 9. Address Review Comments

After submitting your pull request, other contributors may review your code and provide feedback. Address any comments or suggestions by making additional commits to your feature branch. These changes will automatically be added to your pull request.



## 10. After Merging

Once your pull request has been approved and merged, you can safely delete your feature branch:

git checkout main

git pull origin main # to ensure your local main is updated

git branch -d feature-branch-name

git push origin --delete feature-branch-name


Congratulations, you've successfully contributed to the project! Repeat steps 4-11 for future contributions.
