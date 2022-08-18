pipeline {
    agent any
    stages {
       stage('Lint check') {
          steps {
            sh "npm install jslint"
            sh "curl -sL https://rpm.nodesource.com/setup_lts.x |sudo bash"
            sh "ls -lrt node_modules/jslint/bin/"
            sh "~/node_modules/jslint/bin/jslint.js server.js"
          }
       }
    }
}