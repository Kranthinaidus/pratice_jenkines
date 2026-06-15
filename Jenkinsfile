pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/Kranthinaidus/pratice_jenkines.git'
            }
        }

        stage('Check Node & Firebase') {
            steps {
                bat 'node -v'
                bat 'firebase --version'
            }
        }

        stage('Deploy to Firebase') {
    steps {
        bat '"C:\\Users\\user\\AppData\\Roaming\\npm\\firebase.cmd" deploy --non-interactive'
    }
}

        stage('Message') {
            steps {
                echo 'Successfully deployed to Firebase 🚀'
            }
        }
    }
}
