pipeline {
    agent any

    stages {
        stage('Install Python') {
            steps {
                sh '''
                  apt-get update
                  apt-get install -y python3
                '''
            }
        }

        stage('Run Python script') {
            steps {
                sh 'python3 --version'
                sh 'python3 main.py'
            }
        }
    }
}
