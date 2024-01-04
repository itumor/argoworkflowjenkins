pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Add commands to build your project
                echo 'Building..'
                // e.g., sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                // Add commands to test your project
                echo 'Testing..'
                // e.g., sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // Add commands to deploy your project
                echo 'Deploying..'
                // e.g., sh 'deploy-script.sh'
            }
        }
    }

    post {
        always {
            // Add steps to clean up after the pipeline
            echo 'Cleaning up..'
        }

        success {
            // Steps to perform on success
            echo 'Build succeeded!'
        }

        failure {
            // Steps to perform if the pipeline fails
            echo 'Build failed!'
        }
    }
}
