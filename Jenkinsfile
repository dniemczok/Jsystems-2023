pipeline {
    agent none
    stages {
        stage('Check maven version') {
            agent {
                docker { image 'maven:3-alpine' }
            }
            steps {
                sh 'mvn --version'
            }
        }
        stage('Check java version') {
            agent {
                docker { image 'openjdk:8-jre' }
            }
            steps {
                sh 'java -version'
            }
        }
    }
}
