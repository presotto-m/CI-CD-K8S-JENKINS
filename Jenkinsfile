pipeline {
    agent any

    stages {

        stage ('Build Docker Image') {
            steps {
                scrip {
                    docker = docker.build("matheuspresotto/kubectl-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }
        }

    }

}
