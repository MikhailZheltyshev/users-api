#!groovy

pipeline {
    agent { label 'ecs-agent' }

    stages {
        stage('Build') {
            steps {
                sh "./mvnw clean package"
            }
            stage('Test') {
                steps {
                    sh "./mvnw test"
                }
            }
        }
    }
}