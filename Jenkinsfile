pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/JOstapjuk/testProject.git'
            }
        }

        stage('Install') {
            steps {
                script {
                    sh 'npm install'
                }
            }
        }

        stage('Run') {
            steps {
                script {
                    sh 'npm start &'
                }
            }
        }
    }
}
