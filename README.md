# Dependabot Update Script for Azure Devops

This repo is a fork of https://github.com/dependabot/dependabot-script
It is intended to give you a feel for how Dependabot Core works on Azure devops.
Please refer to the above repo for more information.

## Setup and usage

Clone the repo from Github

    git clone https://github.com/rjdkolb/dependabot-script.git

Create a Devops repository `dependabot-script` in the Devops frontend

    git remote add origin git@ssh.dev.azure.com:v3/YOURORG/dependabot-script/dependabot-script
    git push -u devops --all

Create a personal access token in Azure Devops

### Running pipeline with `azure-pipelines.yml`

    * Branch/tag e.g. master
    * The relative path to your project e.g. rjdkolb/mydependabot-exploration
    * Package manager type to scan
    * If you have a custom Azure Devops URL, default value dev.azure.com
    * The secret SECRET_AZURE_ACCESS_TOKEN to access your repo

