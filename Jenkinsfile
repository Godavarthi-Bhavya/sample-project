pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                withMaven(maven : 'MAVEN_HOME') {
                sh 'mvn install -Dmaven.test.skip=true' 
                }
            }
        }
        stage('Sonar') { 
            steps {
                withMaven(maven : 'MAVEN_HOME') {
                sh 'mvn sonar:sonar' 
                } 
            }
        }
    }
}
