pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git branch: 'development', url: 'https://github.com/aamirpatel/GeneralSpringBootProgExce.git'
                sh 'mvn clean install sonar:sonar -Dsonar.password=admin123 -Dsonar.login=admin'
            }
        }
        
         stage('Test') {
            steps {
               echo "Test"
             
            }
        }
    }
}

