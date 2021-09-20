pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 8080:3000'
        }
    }
    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
    }
}