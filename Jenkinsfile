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
	stage('Test1') {
	    steps {
		sh 'python echo_name.py'
            }
            }
    stage('Test2'){
        steps {
        sh 'python web_application_test/test.py'
        }
            }
        }
    }
