pipeline {
    agent none
    stages {
        stage('Build JDK8') {
            agent { docker 'openjdk:8-jdk' }
            steps {
                sh './mvnw verify -fae -Pfast'
            }
        }
    }
}