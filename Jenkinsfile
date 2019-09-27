pipeline {
    agent {
       docker {
            image 'node:7-alpine'
             }
          }
    stages {
      stage('First') {
         steps {
           sh 'pwd'       
           sh 'ls'
           sh 'node hello.js'
          }
        }
       }
   post {
        success {
           cleanWs()
        }
    }
     }
