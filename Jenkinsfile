@Library('roboshop-shared-library@main') _

pipeline {
    agent any
    stages {
       stage('Lint check') {
          steps {
            script{
              sample.info("hello", "preethi.com") 
            }
            sh "echo ******started link check******"
            sh "npm install jslint"
            sh "ls -lrt node_modules/jslint/bin"
            sh "~/node_modules/jslint/bin/jslint.js server.js || true"
            sh "echo ******lint check completed********"
          }
       }
    }
}


