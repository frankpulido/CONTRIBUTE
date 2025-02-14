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
