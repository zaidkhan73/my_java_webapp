pipeline {
    agent any

    stages {
        stage('Checkout SCM') {
            steps {
                // Public repo, credentials not needed
                git branch: 'main', url: 'https://github.com/zaidkhan73/my_java_webapp.git'
            }
        }

        stage('Build') {
            steps {
                // Simple test command
                echo "Build stage: This is just a test. No actual build required."
            }
        }

        stage('Test') {
            steps {
                // Simple test command
                echo "Test stage: Repo checked out successfully!"
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
