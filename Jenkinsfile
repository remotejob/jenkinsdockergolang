pipeline {
    agent {
        docker { image 'golang:1.19-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'ls -trl'
            }
        }
    }
}