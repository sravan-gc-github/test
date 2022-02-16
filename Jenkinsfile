pipeline {
    agent {
        docker { 
               image 'sravangcpdocker/toolkit:11' 
               args '-u root:sudo -v $HOME/workspace/myproject:/myproject'
           }
    }
    stages {
        stage('verison') {
            steps {
                sh '''
                   #!/bin/bash
                   whoami
                   '''
            }
        }
    }
}
