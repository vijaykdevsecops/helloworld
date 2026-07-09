pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/vijaykdevsecops/ci-cd_project.git'
            }
        }
        stage('Build') {
            steps {
                sh 'javac HelloPipeline.java'
            }
        }
        stage('Run') {
            steps {
                sh 'java HelloPipeline from GitHub'
            }
        }
    }
}
