pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                echo "Checking out code..."
                checkout scm
            }
        }
        
        stage('Load Test') {
            steps {
                echo "Навантажувальний тест Jenkins"
                echo "Branch: ${env.BRANCH_NAME}"
                echo "Build: ${env.BUILD_NUMBER}"
                sh '''
                    echo "Running load test on Jenkins agents..."
                    echo "This is a placeholder for load testing logic"
                '''
            }
        }
    }
    
    post {
        always {
            echo "Pipeline completed for branch: ${env.BRANCH_NAME}"
        }
    }
}

