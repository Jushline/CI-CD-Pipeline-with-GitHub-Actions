CI/CD Pipeline with GitHub Actions

This is a simple Python-based project integrated with GitHub Actions to demonstrate how CI/CD automation works. It installs dependencies and simulates a test step on every push or pull request.

What This Project Does

-  Automatically runs a workflow on every `git push` or `pull request` to the `master` branch.
-  Sets up Python 3.9 environment using GitHub-hosted runners.
-  Installs dependencies from `requirements.txt`.
-  Runs a dummy test step to simulate continuous integration.


 File Structure
ci-cd-python-app
 app.py # Sample Python file (optional)
requirements.txt # Python dependencies
.github
workflows
 ci-cd.yml # GitHub Actions workflow file


What I Learned
•	How to create a .github/workflows/ci-cd.yml file to automate CI steps.
•	How to fix issues when the GitHub workflow doesn't trigger (my branch name was master, not main).
•	Difference between GitHub and GitHub Actions.
•	How to debug and fix push errors using Git commands like git pull --rebase, git push -f, etc.

How to Test This Project
1.	Push any code change to the master branch.
2.	Go to the Actions tab in your GitHub repository.
3.	You'll see the pipeline run with  success if everything works.
Final Notes
This is a basic CI/CD setup. No deployment is done in this version — just CI.
To make it full CI/CD:
•	Add build scripts
•	Add deployment steps (e.g., AWS S3, EC2, Heroku, DockerHub)


