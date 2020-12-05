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
		
	        sh 'node ./bin/www'  
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
