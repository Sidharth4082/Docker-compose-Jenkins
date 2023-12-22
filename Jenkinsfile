pipeline {
    agent any

    stages {
	
	    stage('Docker Login') {
		    steps {
			    bat "docker login -u sid2104 -p BaPP4082#@Y docker.io"
			}
        }			
        stage('Deploy') {
            steps {
                bat 'docker-compose up'
            }
        }		
			
    }
}