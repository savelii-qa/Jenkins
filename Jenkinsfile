pipeline {
  agent any

  stages {
    stage('Debug workspace') {
      steps {
        sh '''
          echo "PWD:"
          pwd
          echo "WORKSPACE:"
          echo $WORKSPACE
          ls -la
        '''
      }
    }

    stage('Run Python in Docker') {
      steps {
        sh '''
          docker run --rm \
            -v "$WORKSPACE:/app" \
            -w /app \
            python:3.11-slim \
            python main.py
        '''
      }
    }
  }
}

