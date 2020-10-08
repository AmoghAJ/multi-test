pipeline {
    agent none
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'busybox:latest'
                }
            }
            steps {
                sh 'echo "I am building main01!"'
            }
        }
    }
}
