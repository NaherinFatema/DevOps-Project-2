*Static Website Deployment with AWS S3 and GitHub Actions

This project demonstrates how to deploy a static website using AWS S3 and automate deployments using GitHub Actions. It uses only free-tier services and does not used a custom domain.



Project Overview

* Static HTML and CSS website hosted on AWS S3
* Automated CI/CD pipeline using GitHub Actions
* Publicly accessible via the S3 website endpoint
* No domain name was used
* No paid services required



Project Structure

* index.html
* about.html
* styles.css
* .github/workflows/deploy.yml



Tools Used

* AWS S3 for static website hosting
* GitHub Actions for deployment automation
* GitHub Secrets to store AWS credentials securely
* HTML and CSS for the website content



Setup Instructions

* Clone the repository to your local machine
* Create an S3 bucket with static website hosting enabled
* Upload index.html, about.html, and styles.css to confirm hosting works
* In your GitHub repository, create the following secrets:

  * AWS\_ACCESS\_KEY\_ID
  * AWS\_SECRET\_ACCESS\_KEY
* The IAM user must have permission to upload to the S3 bucket

*GitHub Actions Workflow

* Defined in .github/workflows/deploy.yml
* Automatically runs on every push to the main branch
* Steps:

  * Checkout the code
  * Configure AWS credentials
  * Sync project files to the S3 bucket using "aws s3 sync"



-How to Deploy

* Edit any of the website files
* Commit and push changes to the main branch
* GitHub Actions will automatically upload the updated files to the S3 bucket


-Accessing the Website

The website is live and accessible through the public S3 website endpoint.
A custom domain name was not used.

-Naherin Fatema
