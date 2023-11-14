pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Add build commands here
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add test commands here
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add deployment commands here
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
