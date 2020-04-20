pipeline {
	agent any
	
	stages {
		stage('Clean dir') {
			steps {
				echo 'cleaning directory'
			}
		}
		stage('Build') {
			steps {
				echo 'Build directory'
			}
		}
		stage('Execute Testcase') {
			steps {
				echo 'Executing Testcase'
			}
		}
		stage('Deploy') {
			steps {
				echo 'Deployed Successfully !!'
			}
		}
	}
	post {
		always {
			echo 'One way or another, I have finished' 
		}
		success {
			echo 'I succeeded !!'
		}
	}

}
