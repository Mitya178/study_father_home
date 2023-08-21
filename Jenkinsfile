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
                   echo "Hello, father!" > /opt/file.txt
                '''
            }
        }
    }
}
