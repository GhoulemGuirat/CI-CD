pipeline{
    agent any



    stages {

      stage('debut') {
            steps {
               echo "debut" 
            }
        }
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
          stage('fin') {
            steps {
               echo "fin" 
            }
        }
       }
}




