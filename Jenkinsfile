pipeline {
    agent {
        none
    }
    stages {
        stage('create') {
            steps {
                message 'check, verify'
            }
        }
        stage('build') {
            steps {
                message 'artifacts build'
            }
        }
        stage('deploy') {
            steps {
                message 'deployment'
            }
        }
        stage('test') {
            input {
                message 'About to test the application'
                ok 'Ok'
            }
            steps {
                echo "Check that '${env.PRJ}.${env.DOMAIN}' returns HTTP 200"
                
            }
        }
    }
    
}
