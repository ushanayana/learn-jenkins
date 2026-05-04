pipeline {
    agent {
        label 'AGENT-1'
    }
    options{   //TIMEOUT COUNTER STARTS BEFORE AGENT IS ALLOCATED
        timeout(time: 30, unit: 'SECONDS')
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo "this is build"'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "this is test"'
                sh  'sleep 10'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "this is deploy"'
            }
        }
    }
}