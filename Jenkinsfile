peline{    agent any



    stages {


        stage('Getting project from Git') {
            steps{
      			checkout([$class: 'GitSCM', branches: [[name: '*/master']],
			extensions: [],
			userRemoteConfigs: [[url: 'https://github.com/GhoulemGuirat/CI-CD.git']]])
            }
        }

	stage('Build') {
	            steps {
	                sh 'npm install'
	                sh 'ng build --prod'
	            }
        }
}



