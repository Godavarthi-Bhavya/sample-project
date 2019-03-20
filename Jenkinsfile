pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'mvn install -Dmaven.test.skip=true' 
            }
        }
        stage('Sonar') { 
            steps {
                sh 'mvn sonar:sonar' 
            }
        }
    }
}
