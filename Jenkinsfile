pipeline {
    agent {
        label 'ubuntu-docker-maven'
    }
    stages {
        stage('Build') {
            steps {
                script {
                    docker.image('maven:3.9.6-eclipse-temurin-17-alpine').inside {
                        sh 'mvn --version'
                    }
                }
            }
        }
    }
}
