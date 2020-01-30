pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python:2-alpine' 
                }
            }
        }
	stage('Test') {
	    steps {
		sh 'python echo_name.py'
            }
        }
    }
}
