pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Checkout code from your GitHub repository
                git 'https://github.com/DandySabrrish1999/AndroGoat.git'
            }
        }
        stage('Build') {
            steps {
                // Use gradle to build the project
                bat 'start /B gradle clean build'

            }
        }
        stage('Archive') {
            steps {
                archiveArtifacts artifacts: '**/target/*.jar', allowEmptyArchive: true
            }
        }
    }
}
