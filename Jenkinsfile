@Library('roboshop-shared-library@main') _

pipeline {
    agent any
    stages {
       stage('Lint check') {
          steps {
            script{
              nodejs.lintcheck("cart", "dev") 
            }
          }
       }
    }
}


