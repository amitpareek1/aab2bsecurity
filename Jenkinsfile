pipeline {
	agent { label 'jenkinremotedir'}
	stages {
		stage ('checkout') {
			steps {
			checkout scm
			}
		}
		stage ('build') {
			steps {
				script {
			sh 'npm install'
			}
			}
		}
		stage ('deploy') {
			steps {
				script {
		sh 'cd bin & nohup node www'  
		}
			}
		}
		stage ('test: functional') {
			steps {
			print 'success'
			}
		}
		
	}
}
