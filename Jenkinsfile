pipeline {
    agent {
        docker {
            image 'python:3.11-slim'
        }
    }

    stages {
        stage('Run Python script') {
            steps {
                sh 'python --version'
                sh 'python main.py'
            }
        }
    }
}
