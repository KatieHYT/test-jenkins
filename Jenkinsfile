pipeline {
    agent {
        docker {
            image 'yuting2727/kth_plygnd:191009'
    }
}
    stages {
	    stage('Test1') {
	        steps {
		        sh 'echo 1+2=3HELLO WORLD!!!conflict! merge dev-1'
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
