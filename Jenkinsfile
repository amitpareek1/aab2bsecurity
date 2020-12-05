pipeline {
	agent "jenkinremotedir"
	stages {
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
