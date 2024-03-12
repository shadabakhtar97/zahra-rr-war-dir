pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the repository
                git 'https://github.com/shadabakhtar97/zahra-rr-war-dir.git'
            }
        }
        
        stage('Deploy') {
            steps {
                // Copy the WAR file to Tomcat webapps directory
                sh 'cp SampleWebApp.war /home/ec2-user/apache-tomcat-9.0.86/webapps'
            }
        }
    }
}
