pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/yourname/flask-jenkins-docker.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    docker.build('flask-jenkins')
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    sh 'docker rm -f flask-container || true'
                    sh 'docker run -d -p 5000:5000 --name flask-container flask-jenkins'
                }
            }
        }
    }
}
