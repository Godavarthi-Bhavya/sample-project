pipeline {
    agent any 
    stages {
        tool name: 'MAVEN_HOME', type: 'maven'
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
