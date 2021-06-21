pipeline {
    agent {
        docker {
            image 'openjdk:8-jdk-alpine'
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
        stage('Test') { 
            steps {
                sh 'mvn test'
            }
            post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }
        stage('Deliver') {
            steps {
                sh './jenkins/scripts/deliver.sh'
            }
            post {
                always {
                    echo 'peepee poopoo'
                }
            }
        }
    }
}
