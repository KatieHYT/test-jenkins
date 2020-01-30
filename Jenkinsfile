pipeline {
    agent {
        docker {
            image 'python:3.7.2'
    }
}
    stages {
        stage('Build') { 
	    steps {
                sh 'echo && pwd'
            }
        }
	stage('Test') {
	    steps {
		sh 'python echo_name.py'
            }
        }
    }
}
