pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Start Application') {
            steps {
                bat 'start npm run start'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'npm test'
            }
        }
    }
}
