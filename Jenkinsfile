pipeline {
    agent {
        docker {
            image 'python:3.7.2'
    }
}
    stages {
	    stage('Test1') {
	        steps {
		        sh 'echo HELLO WORLD!'
            }
            }
        stage('Build2') { 
	        steps {
                sh 'pip install -r web_application_test/requirements.txt'
            }
        }
        stage('Test2'){
            steps {
                sh 'python web_application_test/test.py'
        }
            }
        }
    }
