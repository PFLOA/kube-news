pipeline {
    agent any

    stages {
        stage('Build docker image !')
            steps{
                script {
                    dockerapp = docker.build("fabricioveronez/kube-news:${env.BUILD_ID}", '-f ./Dockerfile ./src')
                }
            }
    }
}