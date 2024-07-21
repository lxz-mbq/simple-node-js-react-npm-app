pipeline {
	agent {
		docker {
			image 'node:14-alpine'
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
