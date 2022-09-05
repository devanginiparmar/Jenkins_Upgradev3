pipeline {
    agent any
    stages {
        stage('checkout code') {
            steps {
                sh 'mvn -f java-tomcat-sample/pom.xml clean package'
            }
            post {
                success {
                    echo "Building Application"
                    archiveArtifacts artifacts: '**/*.war'
                }
            }
        }
        stage('Deploy in Staging Environment'){
            steps{
                build job: 'Deploy_App'
 
            }
        }    
    }
}    
        
