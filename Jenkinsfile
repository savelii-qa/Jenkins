pipeline {
  agent any

  stages {
    stage('Run Python in Docker') {
      steps {
        sh '''
          docker run --rm \
            -v "$PWD:/app" \
            -w /app \
            python:3.11-slim \
            python main.py
        '''
      }
    }
  }
}

