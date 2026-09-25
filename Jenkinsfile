pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                bat '"C:\\Users\\HP\\AppData\\Local\\Python\\pythoncore-3.14-64\\python.exe" -m pip install -r requirements.txt'
            }
        }

        stage('Test') {
            steps {
                bat '"C:\\Users\\HP\\AppData\\Local\\Python\\pythoncore-3.14-64\\python.exe" -m pytest'
            }
        }

        stage('Build') {
            steps {
                bat '"C:\\Users\\HP\\AppData\\Local\\Python\\pythoncore-3.14-64\\python.exe" --version'
            }
        }
    }
}