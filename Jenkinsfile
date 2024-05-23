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
                // Use Maven to build the project
                sh 'mvn clean package'
            }
        }
        stage('Archive') {
            steps {
                archiveArtifacts artifacts: '**/target/*.jar', allowEmptyArchive: true
            }
        }
    }
}
