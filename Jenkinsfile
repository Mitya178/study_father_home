pipeline {
    agent any
    stages {
        stage('start') {
            steps {
                sh '''
                   kubectl get pods
                '''
            }
        }
    }
}
