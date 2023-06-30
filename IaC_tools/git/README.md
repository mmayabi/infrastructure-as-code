# Introduction to Git

## What is Git?

- open source
- cross-platform
- **distributed version control system**
- allows to work on the same code simultaneously
- keep track of changes
- collaborate
- revert to previous versions if necessary
- can be installed on local machines for client-side code manipulation, as well as on servers for hosting and managing remote repositories.

Some of remote repositories solutions:

- [GitHub](https://github.com)
- [GitLab](https://gitlab.com)
- [Bitbucket](https://bitbucket.org)
- [GitKraken](https://www.gitkraken.com/)

## Why use Git in IaC?

Because we have **code** and **teams**, I think that Git is a **fundamental** part of all Infrastructure as Code (IaC) architectures.

## Git Installation

In Linux, if you use your distribution's package manager, Git installation is as simple as:

```
apt install git  # Debian
yum install git  # Redhat
```

Before installing Git, it's a good idea to check the [Git-scm](https://git-scm.com/downloads) for any updates or changes to the installation process or software.
for more details, these resources provide helpful manuals and guides:

- chapter 6 of [Learning DevOps](../../IaC_resources/LearningDevOps_MikaelKrief_Packt.md) (especially for Windows)

## Git Terminology

**Repository:** A location where files and codes are stored and managed.

**Clone:**  Create a copy of a remote repository on a local machine.

**Commit:** A saved snapshot of changes made to a repository's files, along with a commit message describing the changes.

**Push:** Uploading the committed changes from a local to a remote repository.

**Pull:** Downloading changes from a remote into a local repository.

**Branch:** A separate copy of a repository's code, where changes can be made without affecting the main codebase.

**Merge:** Combining changes from two or more branches of a repository into a single branch, allowing the changes to be incorporated into the main codebase.

**Fork:** Creating a copy of a repository in order to make changes to it independently.

## Git Commands

```
git clone <url of the remote repository>
git status
git add <files name>
git commit -m "<commit message>"
git push <alias of the remote repository> <branch>
git pull
```

Good resources:

- [Visual Git Cheat Sheet](https://ndpsoftware.com/git-cheatsheet.htm) (highly useful)

## Branch Strategy Patterns

Branch strategy patterns, also known as branching models or branching strategies, are approaches to managing Git branches that help teams to organize their development efforts and simplify their workflows.

TODO: [Git Branching Strategies](https://tilburgsciencehub.com/building-blocks/collaborate-and-share-your-work/use-github/git-branching-strategies/) / [git-scm](https://git-scm.com/book/en/v2/Git-Branching-Branches-in-a-Nutshell) / [atlassian](https://www.atlassian.com/git/tutorials/comparing-workflows)

- Trunk-Based Development:
- Feature Branching:
- Release Branching:
- Git Flow:

    ref: [Git-Flow Github](https://github.com/nvie/gitflow) / [Learning DevOps](../../IaC_resources/LearningDevOps_MikaelKrief_Packt.md) page 186
    
## Learning Resources
