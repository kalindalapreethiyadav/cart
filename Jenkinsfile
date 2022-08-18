pipeline {
    agent any
    stages {
       stage('Lint check') {
          steps {
            sh "~/node_modules/jslint/bin/jslint.js"
            sh "npm install jslint"
            sh "ls -lrt /node_modules/jslint/bin/jslint.js"
          }
       }
    }
}