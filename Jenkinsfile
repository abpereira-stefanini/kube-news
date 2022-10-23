pipeline {
    agent any

    stages {

        stage ('Build Docker Image') {
            steps {
                scrip {
                    dockerapp = docker.build("abpereira/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }
    }

}