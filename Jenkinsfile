pipeline {
    agent any
    tools {
        maven "maven3"
        JDK "OracleJDK8"
    }
    environment{
        NEXUS_USER = 'admin'
        NEXUS_PASS = 'admin'
        RELEASE_REPO = 'vpro-releases'
        CENTRAL_REPO = 'vprofile-maven-central'
        NEXUS_GRP_REPO = 'vprofile-group'
        CENTRAL_REPO = 'maven-central-repo'
        NEXUSIP = '172.31.45.123'
        NEXUSPORT = '8081'
        NEXUS_LOGIN = 'nexuslogin'
    }
    stages{
        stage(Build){
            steps{
                sh 'mvn -s settings.xml -DskipTests install'
            }
        }
    }
}