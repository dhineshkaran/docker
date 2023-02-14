pipeline {
    agent any
    tools {
        maven "maven3"
        jdk "OracleJDK8"
    }
    environment{
        NEXUS_USER = 'admin'
        NEXUS_PASS = 'admin'
        RELEASE_REPO = 'vpro-releases'
        CENTRAL_REPO = 'vprofile-maven-central'
        NEXUS_GRP_REPO = 'vprofile-group'
        NEXUSIP = '172.31.45.123'
        NEXUSPORT = '8081'
        NEXUS_LOGIN = 'nexuslogin'
    }
    stages{
        stage('BUILD'){
            steps {
                sh 'mvn clean install -DskipTests'
            }
        }
    }
}