pipeline {
    agent any 
    tools {
        maven 'MAVEN_HOME'
        //name: 'MAVEN_HOME', type: 'maven'
    }
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
