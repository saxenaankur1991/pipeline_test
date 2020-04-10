pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
		message: "Attention @here ${env.JOB_NAME} #${env.BUILD_NUMBER} has started."
                color: 'RED'
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post {
        always {
            echo 'One way or another, I have finished'
            deleteDir() /* clean up our workspace */
        }
        success {
	    color: 'good'
            message: "The pipeline ${currentBuild.fullDisplayName} completed successfully."
            echo 'I succeeeded!'
        }
        unstable {
            echo 'I am unstable :/'
        }
        failure {
            echo 'I failed :('
        }
        changed {
            echo 'Things were different before...'
        }
    }
}
