pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Kranthinaidus/pratice_jenkines.git'
            }
        }

        stage('List Files') {
            steps {
                bat 'dir'
            }
        }

        stage('Message') {
            steps {
                echo 'Pipeline is running successfully'
            }
        }
    }
}