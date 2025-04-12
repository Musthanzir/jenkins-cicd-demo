pipeline {
    agent any  // Use any available agent (master or slave)

    stages {
        stage('Build') {
            steps {
                script {
                    echo "Building the project"
                    // Example build command (you can replace with your actual build process)
                    bat 'echo Build successful'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    echo "Running tests"
                    // Example test command (replace with your actual test process)
                    bat 'echo Tests passed'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    echo "Deploying to staging environment"
                    // Example deploy command (replace with your actual deploy process)
                    bat 'echo Deployment successful'
                }
            }
        }
    }

    post {
        always {
            echo "Pipeline finished"
        }
        success {
            echo "Pipeline completed successfully"
        }
        failure {
            echo "Pipeline failed"
        }
    }
}
