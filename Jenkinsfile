pipeline {
    agent {
        docker { image 'sravangcpdocker/toolkit:11' }
    }
    stages {
        stage('verison') {
            steps {
                sh '''
                   #!/bin/sh
                   ping -c 5 192.168.1.4
                   '''
            }
        }
    }
}
