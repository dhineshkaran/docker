pipeline{
    agent any
    stages{
        stage('GitCheckout'){
            git branch: 'main', credentialsId: 'gitcredentials', url: 'https://github.com/dhineshkaran/docker.git'
        }
        stage('build'){
            sh 'mvn install'
        }
    }
}