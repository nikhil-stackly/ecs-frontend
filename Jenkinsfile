pipeline {
  agent any

  stages {

    stage('Build Docker Images') {
      steps {
        sh '''
          echo "Building backend image"
          docker build -t backend backend/

          echo "Building frontend image"
          docker build -t frontend frontend/
        '''
      }
    }

  }
}
