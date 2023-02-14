pipeline{
    agent any
    stages{
        stage('GitCheckout') {
            steps {
                git branch: 'main', credentialsId: 'gitcredentials', url: 'https://github.com/dhineshkaran/docker.git'
            }
    }   }
}