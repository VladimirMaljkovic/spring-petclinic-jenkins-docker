pipeline {
    agent {
        docker {
            image 'openjdk:8-jdk-alpine'
        }
    }
    stages {
        stage('Testing') { 
            steps {
                sh 'echo printing'
                sh 'ls'
            }
        }
        
    }
}
