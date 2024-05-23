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
                // Build steps go here, for example:
                 bat 'echo "Build stage running..."'
            }
        }
    }
}
