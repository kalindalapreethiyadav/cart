pipeline {
    agent any
    stages {
       stage('Lint check') {
          steps {
            sh "curl -sL https://rpm.nodesource.com/setup_lts.x | bash"
            sh "npm install jslint"
            sh "ls -lrt node_modules/jslint/bin/"
            sh "~/node_modules/jslint/bin/jslint.js server.js"
          }
       }
    }
}