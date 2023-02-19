pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES1UG20CS427-1 PES1UG20CS427.cpp'
            }
        }
        
        stage('Test') {
            steps {
                sh './PES1UG20CS427-1'
            }
        
        
        stage('Deploy') {
            steps {
                // Add deployment steps here
                echo 'Deploying....'
            }
        }
    }
    
    post {
        always {
            echo 'Pipeline completed'
        }
        
        failure {
            echo 'Pipeline failed'
        }
    }
}
