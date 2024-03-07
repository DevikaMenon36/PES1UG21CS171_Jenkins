pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Placeholder build step
                sh 'echo "Placeholder build step"'
                echo 'Build Stage Successful'
            }
        }
        stage('Test') {
            steps {
                // Placeholder test step
                sh 'echo "Placeholder test step"'
                echo 'Test Stage Successful'
                // Add post condition for test results if needed
            }
        }
        stage('Deploy') {
            steps {
                // Placeholder deploy step
                sh 'echo "Placeholder deploy step"'
                echo 'Deploy Successful'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
