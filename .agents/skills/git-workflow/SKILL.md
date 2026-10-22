\---

name: git-workflow

description: Enforces safe team Git workflow, branches, commits, pull requests, and main-branch protection.

\---



\# Git Workflow



\## Branches



main = stable



develop = integration



feature/\* = individual development



qa/\* = testing



\## Never



\- force push main

\- directly commit main

\- delete another developer's branch

\- reset shared branches without approval



\## Before commit



Run:



\- tests

\- lint

\- build/type check



\## Commit format



Use:



feat:

fix:

test:

refactor:

docs:

chore:



Example:



feat: add user authentication



\## Before push



Check:



git status

git diff

git branch



Ensure no secrets are included.



\## Pull Request



Every PR must describe:



\- what changed

\- why

\- affected components

\- tests performed

\- API changes

\- database changes



\## Main



main only accepts tested changes.

