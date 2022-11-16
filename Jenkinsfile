node {
    checkout scm

    docker.withRegistry('hub.docker.com', 'docker-hub') {

        def customImage = docker.build("jenkinsdockergolang")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}

// pipeline {
//     // agent {
//     //     docker { image 'golang:1.19-alpine' }
//     // }
//     agent { dockerfile true }
//     stages {
//         stage('Test') {
//             steps {
//                 sh 'ls -trl'
//             }
//         }
//     }
// }