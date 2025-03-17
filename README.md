GitHub Deployment Workflow Project

This project is designed to help you understand the concepts of Continuous Integration (CI) and Continuous Deployment (CD) using GitHub Actions. The goal is to create a simple workflow that automatically deploys a static website to GitHub Pages whenever changes are made to the index.html file.
Project Overview

The repository contains:

    A simple index.html file that displays "Hello, GitHub Actions!".

    A GitHub Actions workflow file (deploy.yml) in the .github/workflows directory.

    A README.md file explaining the project and its purpose.

The workflow is triggered whenever changes are pushed to the main branch, specifically when the index.html file is modified. The website is then automatically deployed to GitHub Pages.
Requirements

    A GitHub repository named gh-deployment-workflow (or any name of your choice).

    A simple index.html file 

    A GitHub Actions workflow file (deploy.yml) in the .github/workflows directory to automate the deployment process.

    A README.md file explaining the project.

Workflow File (deploy.yml)

The workflow is defined in the .github/workflows/deploy.yml file. 
Explanation of the Workflow:

    Trigger: The workflow runs on every push to the main branch.

    Jobs:

        Checkout code: Fetches the latest code from the repository.

        Deploy to GitHub Pages: Uses the actions/deploy-pages@v4 action to deploy the website to GitHub Pages.

How It Works

    When you push changes to the main branch, GitHub Actions automatically triggers the workflow.

    The workflow checks out the code and deploys it to GitHub Pages.

    The website is then accessible at the GitHub Pages URL for the repository, e.g., https://<username>.github.io/gh-deployment-workflow/.

Accessing the Website

Once the workflow runs successfully, your website will be live at:
https://<username>.github.io/gh-deployment-workflow/

Replace <username> with your GitHub username and gh-deployment-workflow with the name of your repository.
Steps to Reproduce

    Create a GitHub Repository:

        Create a new repository on GitHub (e.g., gh-deployment-workflow).

    Add Files:

        Add the index.html file with the provided content.

        Create a .github/workflows directory and add the deploy.yml file.

    Push to GitHub:

        Push the files to the main branch of your repository.

    Check GitHub Actions:

        Go to the Actions tab in your repository to see the workflow running.

    Access GitHub Pages:

        Once the workflow completes, visit the GitHub Pages URL to see your deployed website.

Conclusion

This project demonstrates how to use GitHub Actions to automate the deployment of a static website to GitHub Pages. It introduces the concepts of Continuous Integration and Continuous Deployment, which are essential for modern software development workflows.

https://roadmap.sh/projects/github-actions-deployment-workflow