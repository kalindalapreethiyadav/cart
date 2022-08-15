pipeline{
    agent any
    stages{
             stage ('lint check') {
                 steps {
                    sh "echo installing jslint"
                    sh "curl -sL https://rpm.nodesource.com/setup_lts.x |sudo bash"
                    sh "npm install jslint"
                    sh "ls -lrt node_modules/jslint/bin"
                    sh "~/node_modules/jslint/bin/jslint.js server.js || true"
                    sh "echo completed lint check"
                 }
             }
    }
    }