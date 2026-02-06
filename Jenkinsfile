pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code already checked out from SCM'
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

