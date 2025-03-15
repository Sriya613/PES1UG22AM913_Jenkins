pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                script {
                    sh 'git clone https://github.com/Sriya613/PES1UG22AM913_Jenkins.git'
                }
            }
        }
        
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o PES1UG22AM913-1 main.cpp'
                }
            }
        }
        
        stage('Test') {
            steps {
                script {
                    sh './this_file_does_not_exist'
                }
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
