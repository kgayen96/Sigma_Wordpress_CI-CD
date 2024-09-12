# Sigma_Wordpress_CI-CD
Pre-requisites:
GitHub Repository: The code (including Dockerfile, docker-compose.yml, and the GitHub Actions workflow) must be pushed to a GitHub repository.

#**Steps to Set Up:****
1. Clone the Repository:
    Clone the repository with your project files to the machine where you want to deploy or test locally
    $ git clone https://github.com/kgayen96/Sigma_Wordpress_CI-CD.git

2. Create the GitHub Actions Workflow:
    The GitHub Actions workflow ci-cd.yml is already set up in your repository under .github/workflows/. This file automates the process of building and deploying Docker containers.

3. Run the Pipeline:
    When code is pushed to the main branch or a pull request is created, the pipeline is automatically triggered by GitHub Actions.

4. Verify WordPress and MySQL Services:
    The pipeline includes a verification step (curl) that checks whether WordPress is running on http://localhost:8080. If the pipeline succeeds, WordPress and MySQL are both up and running         within Docker containers.
