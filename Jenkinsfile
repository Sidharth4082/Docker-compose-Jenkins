pipeline {
    agent any

    stages {
	
	    stage('Docker Login') {
		    steps {
			    bat "docker login -u <docker-user id> -p <docker-hub password> docker.io"
			}
        }			
        stage('Deploy') {
            steps {
                bat 'docker-compose up'
            }
        }		
			
    }
}
