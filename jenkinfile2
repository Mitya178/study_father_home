pipeline {
  agent {
    kubernetes {
      label 'test-mp2'
      defaultContainer 'ssh-client'
      cloud 'kubernetes'
      yaml """
        apiVersion: v1
        kind: Pod
        spec:
          containers:
          - name: ssh-client
            image: docksal/ssh-agent:edge
            command:
            - cat
            tty: true
          imagePullSecrets:
          - name: artifactory-pro
        """.stripIndent()
    }
  }

  stages {
      stage('Hello') {
          steps {
              sh '''
                echo 'Hello World'
                echo 1-`date`
                echo 2-`date`
                echo 3-`date`
                echo 7-`date`
              '''
          }
      }
  }
}
