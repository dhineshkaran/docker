pipeline{
    stages {
    stage('Git checkout SCM') 
    steps{
          git branch: 'main', credentialsId: 'gitcredentials', url: 'https://github.com/dhineshkaran/docker.git'
      }
    stage('Build project')
    steps{
        sh 'mvn clean install -DskipTests'
    }   
  }
}