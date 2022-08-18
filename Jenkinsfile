pipeline {
    agent { label 'java' }
    stages {
       stage('Lint check') {
          steps {
            sh "started lint check"
            sh "npm install jslint"
            sh "ls -lrt node_modules/jslint/bin/"
            sh "~/node_modules/jslint/bin/jslint.js server.js"
          }
       }
    }
}