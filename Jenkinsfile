pipeline {
    // agent {
    //     docker { image 'golang:1.19-alpine' }
    // }
    agent { dockerfile true }
    stages {
        stage('Test') {
            steps {
                sh 'ls -trl'
            }
        }
    }
}