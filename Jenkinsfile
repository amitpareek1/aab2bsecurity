pipeline {
	agent { label 'jenkinremotedir'}
	stages {
		stage ('checkout') {
			checkout scm
		}
		stage ('build') {
			sh 'npm install'
		}
		stage ('deploy') {
		sh 'cd bin & nohup node www'  
		}
		stage ('test: functional') {
			print 'success'
		}
		
	}
}
