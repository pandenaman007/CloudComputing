
pipeline {
	agent any
	stages {
		stage('clone') {
			steps {
				git branch : "main",
				url : "https://github.com/pandenaman007/CloudComputing"
			}
		}
		stage('build') {
			steps {
				make -C main
			}
		}
		stage('test') {
			steps {
				/var/jenkins_home/workspace/PES2UG20CS210-1/main/hello_exec
			}
		}
	}
	post{
		failure{
			echo "failed pipeline"
		}
	}
}


