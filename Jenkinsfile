pipeline {
    agent { label 'ecs-agent' }

    stages {
        stage('Build') {
            sh './mvnw clean package'
        }
        stage('Test') {
            sh './mvnw test'
        }
    }
}