pipeline {
    agent any
    stages {
		stage("Checkout"){
			steps{
				checkout([$class: 'GitSCM',
					branches:[[name: 'master']]
					userRemoteConfigs: [[credentialsId: '24908372-4b9d-4fa0-8eaa-179d3e145cc5',
					url: 'https://github.com/RashmiNema/Multibranch-dmo.git']]])
			}
		}
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
            }
       }
	}
}
