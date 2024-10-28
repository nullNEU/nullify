# Contribution guide

## Prerequisites

The following need to be installed on your system to get the site running locally
- Go (`v1.20.x` or above) [More details](https://go.dev/)
- Git [More details](https://git-scm.com/)
- Hugo (Follow instructions on the [official documentation to install hugo](https://gohugo.io/installation/))

## Local setup
- Create a fork of the GitHub repository from your account
  ```bash
  git clone https://github.com/<your-github-username>/nullify
  ```
- Assuming you have hugo installed at this point, you should be able to run the site as below
  ```bash
  hugo server
  ```
- Navigate to `http://localhost:1313` on your browser to see the website in action.

## Taking up an issue
All issues about this project are tracked as [GitHub issues on this repository](). Once you have a fair idea of what tasks have been completed, what are in progress, and what are planned, you can go ahead and pick an issue to work on.

### Some helpful tips
- If you are a beginner, you might want to check issues marked with a [*good first issue*](https://github.com/nullNEU/nullify/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) tag.
- Once you decide on what you want to work on, let the maintainers of the project know that you are interested in working on it by commenting on the issue.

## Opening a PR
Once you have the project setup and running on your system, you can start contributing to it.
- Create a new branch on your local system
> [!IMPORTANT]
> Please ensure that you create a separate branch (from `main`) on your fork for each contribution and name it appropriately (not `main`) since it makes reviewing code easier.
  ```bash
  git checkout -b <your-branch-name> # creates a new branch and switches to it
  ```
- Make sure you figure out what issue you are working on!
- Go through the [project wiki](https://github.com/nullNEU/nullify/wiki) to understand the directory structure of the project and how you can make code, design, data, documentation or other changes.
- Once all your changes are done, commit them to your local branch
  ```bash
  git add . # adds all changed files to the commit
  git commit -m <your-commit-message> # creates a new commit with your commit message
  ```
> [!IMPORTANT]  
> Make sure to include a helpful commit message. 
> - A good commit message is clear, concise and conveys what the commit changes
> - Try writing commit messages in the imperative, i.e. *Add new page* and *Fix bug* instead of *Added new page* and *Fixes many bugs*
- Push it to your fork of the repository
  ```bash
  git push --set-upstream origin <your-branch-name>
  ```
- Go to the branch on your repository on GitHub. There should be an option that says *Open Pull Request*. 
  - This creates a new PR to the `main` branch of the original repository (by default).
  - Make any changes to the title/description as required
- Wait for someone to review your PR and merge it
  - If any changes are requested, please complete them as required.
  - Once the changes look good to the maintainers, they will be merged to the `main` branch!
- You can expect to see your changes live within a few minutes of the PR being merged :)

## Reach out
If you are stuck at any point, feel free to reach out to us on our [Telegram channel](https://t.me/+S7uxWGwmLfY5NTk1).
