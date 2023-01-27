pipeline{
    agent any

    stages{
        stage ('Build Docker Image'){
            steps{
                script{
                    dockerapp = docker.build("jean-rnascimento/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./scr')
                }
            }
        }
    }   
}