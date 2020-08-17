pipeline {
    agent any
    stages {
        stage('---clean---') {
            
            tools {
                maven 'Maven'
                }
            
            steps {
                sh "mvn clean"
                sh "mvn --version"
            }
        }
        stage('--test--') {
            
            tools {
                maven 'Maven'
                }
            
            steps {
                sh "mvn test"
            }
        }
        stage('--package--') {
            
            tools {
                maven 'Maven'
                }
            
            steps {
                sh "mvn package"
            }
        }
    }
}
