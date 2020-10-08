pipeline {
    agent none
    stages {
        stage('Build') {
            when { anyOf 
                    {  branch 'master'; 
                       branch 'prod' } }
            agent {
                docker {
                    image 'busybox:latest'
                }
            }
            steps {
                sh 'echo "I am building!"'
            }
        }
    }
}
