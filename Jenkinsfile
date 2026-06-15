pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Kranthinaidus/pratice_jenkines.git'
            }
        }

        stage('Install Firebase CLI') {
            steps {
                bat 'npm install -g firebase-tools'
            }
        }

        stage('Deploy to Firebase') {
            steps {
                bat 'firebase deploy --non-interactive --token $FIREBASE_TOKEN'
            }
        }

        stage('Message') {
            steps {
                echo 'Deployed to Firebase successfully'
            }
        }
    }
}
