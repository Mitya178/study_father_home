pipeline {
    agent any

    stages {
        //def ci
        stage('pipeline-test1') {
            //container('docker') {
            //  ci.build()
            //}
            steps {
                //container('docker')
                sh '''
                   sudo echo "Hello, father!" > /opt/file.txt
                '''
            }
        }
    }
}
