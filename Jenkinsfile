pipeline {
    agent {
        docker { image 'bitnami/kubectl' }
    }
    stages {
        stage('verison') {
            steps {
                sh '''
                   #!/bin/bash
                   kubectl --version
                   '''
            }
        }
    }

post {
        always {
            cleanWs deleteDirs: true
        }
     }
}
