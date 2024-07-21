pipeline {
	agent {
		docker {
			image 'node:6-alpine'
			registryUrl 'https://registry.npmmirror.com'
			args '-p 3000:3000'
		}
	}
	stages {
		stage('Build') {
			steps {
				sh 'npm install'
			}
		}
	}
}
