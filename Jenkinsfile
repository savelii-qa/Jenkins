pipeline {
  agent any

  stages {
    stage('Run Python in Docker') {
      steps {
        script {
          docker.image('python:3.11-slim').inside {
            sh 'ls -la'
            sh 'python main.py'
          }
        }
      }
    }
  }
}

