node('centos7') {
    stage('checkout code') {
        checkout([$class: 'GitSCM', branches: [[name: 'master']], extensions: [], userRemoteConfigs: [[credentialsId: 'github', url: 'git@github.com:nananoam123/PythonFlask-JobBoard.git']]])
}
 stage('build') {
     sh 'docker build -t flask .'
     
 }
}