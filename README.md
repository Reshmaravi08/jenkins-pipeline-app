# jenkins-pipeline-app

CI/CD pipeline using Jenkins, Docker, and AWS Free Tier. Jenkins runs on an EC2 instance and pulls code from GitHub when changes are pushed. It then builds a Docker image from a Flask app and runs it inside a container on the same EC2. I automated the entire flow using a declarative Jenkinsfile, and configured GitHub webhooks for auto-deploy.

<img width="458" alt="image" src="https://github.com/user-attachments/assets/e3e7140c-c5b6-47f1-9ce1-367545738a09" />


