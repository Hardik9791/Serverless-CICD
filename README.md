# Serverless-CICD
This project demonstrates the creation of a fully automated CI/CD pipeline to deploy a static website using Amazon Web Services (AWS). The website is hosted on Amazon S3 with automated builds and deployments triggered by code changes in a GitHub repository, managed through AWS CodePipeline and AWS CodeBuild.

# Project Architecture
![CICD Pipeline](https://github.com/user-attachments/assets/0d5b9401-b0f2-4ca3-955a-d176eef81c1f)


# Project Features
• Automated Deployments: The pipeline automatically builds and deploys the website whenever there is a new commit to the GitHub repository.
• No Servers to Manage: Since the website is hosted on S3 and deployed using CodePipeline, you don't need to manage any infrastructure.
• Scalable and Cost-Effective: S3 provides virtually unlimited scalability, and you only pay for the storage and bandwidth you use.

# Technologies Used
1. Amazon S3: Hosts the static website and serves it over the internet.
2. AWS CodePipeline: Automates the build, test, and deploy process.
3. AWS CodeBuild: Executes the build process and packages the website files.
4. AWS CodeDeploy: Deploys the website files to S3 bucket.
5. GitHub: Stores the website's source code and triggers pipeline executions on new commits.

# How the Project Works
1. Source Code: The static website’s source code (HTML, CSS, JavaScript) is stored in a GitHub repository.
2. Pipeline Trigger: When changes are pushed to the GitHub repository, the CodePipeline is automatically triggered to start the deployment process.
3. Build Process:
    • AWS CodeBuild packages the static website files based on the instructions defined in the buildspec.yml file.
    • The files are prepared for deployment, ensuring that the static assets (HTML, CSS, JS) are correctly bundled.
4. Deployment:
    • The packaged files are deployed to Amazon S3, where they are made publicly accessible.
    • Proper deployment configuration ensures that all files are extracted and placed in the root of the S3 bucket, making the website accessible.
5. Accessing the Website: Users can access the website via the S3 website endpoint, which serves the static files directly over the web.

# Skills Highlighted
• AWS Services Expertise: Demonstrated proficiency in AWS S3, CodePipeline, and CodeBuild, effectively automating the deployment process for a static website.
• Problem Solving: Identified and resolved issues with file extraction and deployment paths, ensuring the static website was accessible post-deployment.CI/CD Pipeline
• Automation: Set up a fully automated CI/CD pipeline, showcasing knowledge of continuous integration and deployment processes using AWS services.
• GitHub Integration: Successfully integrated GitHub with CodePipeline to trigger automatic deployments based on new commits, highlighting proficiency in version control and source management.
