pipeline{
    agent any



    stages {

        stage('Getting project from Git') {
            steps{
      		deleteDir()
        	checkout scm
            }
        }

	stage('Build') {
	            steps {
	                sh 'npm install'
	                sh 'ng build --prod'
	            }
        }
       }
}




