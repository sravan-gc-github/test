pipeline {
    agent {
        docker { image 'bitnami/kubectl:latest' }
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
