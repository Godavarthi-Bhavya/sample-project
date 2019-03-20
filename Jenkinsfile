pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                withEnv(['MAVEN_HOME=C:\\Program Files\\apache-maven-3.6.0']) {
                // some block
                sh 'mvn install -Dmaven.test.skip=true' 
                }
            }
        }
        stage('Sonar') { 
            steps {
                withEnv(['MAVEN_HOME=C:\\Program Files\\apache-maven-3.6.0']) {
                // some block
                sh 'mvn sonar:sonar'
                }
            }
        }
    }
}
