pipeline {
	agent any
		stages {
			stage('One') {
				steps {
                    echo 'Hi, this is ankur saxena'
					}
                }
                stage('Two') {
					steps {
						input('Do you want to proceed?')
					}
                }
                stage('Three') {
					when {
						not {
                            branch "master"
                       }
					}
				}	
                stage('Four'){
                    steps {
						echo 'Hi, this is ankur saxena'
					}
                 }
        
               }
}
