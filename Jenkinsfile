pipeline {
    agent { label 'master' }
    
    stages {
        stage('create') {
            steps {
                echo 'check, verify'
            }
        }
        stage('build') {
            steps {
                echo 'artifacts build'
            }
        }
        stage('deploy') {
            steps {
                echo 'deployment'
            }
        }
        stage('test') {
            input {
                echo 'About to test the application'
                ok 'Ok'
            }
            steps {
                echo "Check that '${env.PRJ}.${env.DOMAIN}' returns HTTP 200"
                
            }
        }
    }
    
}
