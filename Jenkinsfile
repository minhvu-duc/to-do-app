pipeline {
    agent any
    
    stages {
        stage('Stage 1') {
            steps {
                echo "Running Stage 1"
            }
        }
        
        stage('Stage 2') {
            steps {
                echo "Running Stage 2"
            }
        }
        
        stage('Stage 3') {
            steps {
                echo "Running Stage 3"
            }
        }
    }
    
    post {
        success {
            echo "Pipeline completed successfully!"
        }
        failure {
            echo "Pipeline failed!"
        }
    }
}
