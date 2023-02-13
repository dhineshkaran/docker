pipeline { 
    agent any  
    stages { 
        stage('Git checkout SCM') {
          git branch: 'main', credentialsId: 'gitcredentials', url: 'https://github.com/dhineshkaran/docker.git'
      }
        stage('Build') { 
            steps { 
               sh 'mvn install' 
            }
        }
    }
}