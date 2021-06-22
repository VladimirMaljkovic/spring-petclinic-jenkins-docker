pipeline {
    agent {
        docker
    }
    stages {
        stage('Building artifacts and what not') { 
            steps {
                sh 'echo starting build'
                sh './mvnw package'
            }
        }
        stage('Creating docker container') {
            steps {
                sh 'echo creating docker image...'
                sh 'docker build -t petclinic-docker .'
                sh 'creating docker container...'
                sh 'docker run --rm -p 8888:8080 petclinic-docker'
            }
        }
        
        
    }
}
