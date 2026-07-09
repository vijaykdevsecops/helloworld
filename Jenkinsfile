pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/vijaykdevsecops/helloworld.git'
            }
        }
        stage('Build') {
            steps {
                bat 'javac HelloPipeline.java'
            }
        }
        stage('Run') {
            steps {
                bat 'java HelloPipeline'
            }
        }
    }
}

