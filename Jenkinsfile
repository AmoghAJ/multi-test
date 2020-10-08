pipeline {
    agent none
    stages {
        stage('Build') {
            agent {
                docker {
                    image 'busybox:latest'
                }
            }
            when { anyOf 
                    {  branch 'master'; 
                       branch 'prod' } }
            steps {
                sh 'echo "I am building!"'
            }
        }
    }
}
