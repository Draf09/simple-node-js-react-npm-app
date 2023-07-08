pipeline {
	stages {
		stage('Build') {
			steps {
				sh 'npm install'
			}
		}
	}
	agent {
		docker {
			image 'node:lts-bullseye-slim'
			args '-p 3005:3005'
			}
		}
	}
