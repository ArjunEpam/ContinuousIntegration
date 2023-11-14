pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building the project...'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Running tests...'
          }
        }

        stage('API Tests') {
          steps {
            echo 'Commands for API Tests'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying the application...'
      }
    }

  }
  post {
    success {
      echo 'Pipeline completed successfully! Ready for production.'
    }

    failure {
      echo 'Pipeline failed. Review and address the issues.'
    }

  }
}