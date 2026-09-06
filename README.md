FSD Module 24 — RA 24.2: Test and Deploy an Application Using GitHub Actions
This repository is my submission for Required Assignment 24.2. It demonstrates
setting up a GitHub Actions workflow to test and deploy an application, following
the Quickstart for GitHub Actions
guide.
Learning Outcome
Set up GitHub Actions — create a workflow, develop the steps, run it, and monitor its
execution in the Actions log.
What's in this repository
Path	Purpose
`.github/workflows/github-actions-demo.yml`	The GitHub Actions workflow for this assignment
`README.md`	This file
The workflow
The workflow lives at `.github/workflows/github-actions-demo.yml` and runs
automatically on every `push` to the repository. It runs on a GitHub-hosted
`ubuntu-latest` runner and performs the following steps:
Prints messages showing the event, runner OS, branch, and repository (using GitHub
Actions context variables).
Checks out the repository code onto the runner (`actions/checkout`) so later
steps can access the files.
Lists the files in the repository to confirm the checkout succeeded.
Reports the job's final status.
How to run it
The workflow is triggered automatically whenever code is pushed to the repository. To
view a run:
Go to the Actions tab of this repository.
Select the most recent workflow run (named "GitHub Actions Demo").
Open the Explore-GitHub-Actions job and expand any step to view its log output.
Author
Mitchell Brown (@mbrow121)
