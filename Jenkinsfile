pipeline {
    agent {
        docker { image 'sravangcpdocker/toolkit:11' }
    }
    stages {
        stage('verison') {
            steps {
                sh '''
                   #!/bin/sh
                   whoami
                   '''
            }
        }
    }
}
