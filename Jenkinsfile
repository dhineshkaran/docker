pipeline{
    agent none
    stages{
        stage(GitCheckout){
            git branch: 'main', credentialsId: 'gitcredentials', url: 'https://github.com/dhineshkaran/docker.git'
         }
    }
}