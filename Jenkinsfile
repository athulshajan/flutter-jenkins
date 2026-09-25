pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                bat 'flutter pub get'
            }
        }

        stage('Test') {
            steps {
                bat 'flutter test'
            }
        }

        stage('Build') {
            steps {
                bat 'flutter build apk --debug'
            }
        }
    }
}