pipeline {
    agent any

    tools {
        maven 'maven'
    }

    stages {
        stage('Build') {
            steps {
                git branch: 'development', url: 'https://github.com/aamirpatel/GeneralSpringBootProgExce.git'
                sh 'mvn clean install sonar:sonar -Dsonar.password=admin123 -Dsonar.login=admin'
                sh 'mvn clean package'
            }
        }
        
         stage('Test') {
            steps {
               echo "Test"
             
            }
        }
    }
}


