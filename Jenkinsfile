
 pipeline {
    agent any
    parameters{
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')
        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')
        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
            }
        
            stages {
                stage('Hello') {
                    steps {
                        echo 'Hello World'
                    }
                }
        
                stage('stage two') {
                    steps {
                      echo "I am learning Jenkins"
                      echo "CI & CD"
                      echo "For DevOPs"   
                    }
                }
        
                stage('stage three') {
                    environment{
                Env_url = "preethi.local.com"
            }
                    steps {
                       sh "echo Env_url : $Env_url"
                       sh "env"
                    }
                }
            }
        }