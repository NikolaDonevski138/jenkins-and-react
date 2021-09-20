pipeline {
    agent {
        docker {
            image 'node'
            args '-p 4055:4055'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
    }
}