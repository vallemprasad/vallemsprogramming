pipeline {
    agent { docker { image 'maven:3.9.9-eclipse-temurin:11-jdk' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
