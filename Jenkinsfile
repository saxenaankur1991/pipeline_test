node {
 	// Clean workspace before doing anything
    deleteDir()

    try {
        stage ('Clone') {
        	steps {
                    echo 'Hi, this is ankur saxena'
					}
        }
        stage ('Build') {
        	steps {
                    echo 'Hi, this is ankur saxena'
					}
        }
        stage ('Tests') {
	        steps {
                    echo 'Hi, this is ankur saxena'
					}
        }
      	stage ('Deploy') {
            steps {
                    echo 'Hi, this is ankur saxena'
					}
      	}
    } catch (err) {
        currentBuild.result = 'FAILED'
        throw err
    }
}
