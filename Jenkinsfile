pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python:2-alpine' 
                }
            }
            steps {
                sh 'python -c "print(1)"' 
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Testing!"'
            }
        }
    }
}
