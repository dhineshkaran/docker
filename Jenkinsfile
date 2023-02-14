pipeline {
    agent any
    tools {
        maven "maven3"
        JDK "OracleJDK8"
    }
    stages{
        stage(Build){
            steps{
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }
    }
}