pipeline {
    agent any

    stages {

        stage('Configure Flutter') {
            steps {
                bat 'git config --system --add safe.directory C:/src/flutter'
            }
        }

        stage('Check Flutter') {
            steps {
                bat 'C:\\src\\flutter\\bin\\flutter.bat --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'C:\\src\\flutter\\bin\\flutter.bat pub get'
            }
        }

        stage('Test') {
            steps {
                bat 'C:\\src\\flutter\\bin\\flutter.bat test'
            }
        }

        stage('Build') {
            steps {
                bat 'C:\\src\\flutter\\bin\\flutter.bat build apk --debug'
            }
        }
    }
}