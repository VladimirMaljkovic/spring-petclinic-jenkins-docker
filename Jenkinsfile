pipeline {
    agent any
    stages {
        stage('clearing up docker images') {
            steps {
                sh 'docker ps'
            }
        }
        // stage('Building artifacts and what not') { 
        //     steps {
        //         sh 'echo starting build'
        //         sh './mvnw package'
        //     }
        // }
        // stage('Initialize docker') {
        //     steps {
        //         def dockerHome = tool 'docker'
        //         env.PATH = "${dockerHome}/bin:${env.PATH}"
        //     }
        // }
        // stage('Creating docker container') {
        //     steps {
        //         sh 'echo creating docker image...'
        //         sh 'docker build -t petclinic-docker .'
        //         sh 'echo creating docker container...'
        //         sh 'docker run --rm -p 8888:8080 petclinic-docker'
        //     }
        // }
        
        
    }
}
