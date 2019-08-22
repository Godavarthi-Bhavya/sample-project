pipeline {
    
 agent any {   
    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install -DskipTests'
            }
        }
        stage('Test') {
            steps {
                echo 'in testing stage'
            }
        }

       stage('Sample') {
            steps {
                echo 'in sample stage'
            }
        }
    }
 }
}
