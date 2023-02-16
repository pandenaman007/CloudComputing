
pipeline {
	agent any
	stages{
		stage('Build'){
			steps{
				sh 'g++ -o app PES2UG20CS210.cpp'
			}
		}
		stage('Test'){
			steps{
				sh './app'	
			}
		}
		stage('Deply'){
			steps{
				sh 'Echo its done'
			}
		}
		
	}
	post{
		failure{
			echo 'Partition Failure'
		}
	}
}


