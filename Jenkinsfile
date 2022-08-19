pipeline {
    agent any
    stages {
       stage('Lint check') {
          steps {
            sh "echo started link check"
            sh "npm install jslint"
            sh "ls -lrt sh node_modules/jslint/bin/"
            sh "~/node_modules/jslint/bin/jslint.js server.js"
          }
       }
    }
}


