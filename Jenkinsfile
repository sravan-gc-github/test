pipeline {
    agent {
        docker { image 'rancher/kubectl:v1.23.3' }
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
