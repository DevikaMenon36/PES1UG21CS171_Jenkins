pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Compile the .cpp file using shell script
                sh 'g++ -o PES1UG21CS171-1 PES1UG21CS171.cpp'
            }
        }
        stage('Test') {
            steps {
                // Execute the compiled executable and print its output
                sh './PES1UG21CS171-1'
            }
        }
    }
    
    post {
        always {
            // Display 'pipeline completed' regardless of outcome
            echo 'Pipeline completed!'
        }
        // Check if any of the stages failed
        failure {
            // Display 'pipeline failed' in case of failure
            echo 'Pipeline failed!'
        }
    }
}
