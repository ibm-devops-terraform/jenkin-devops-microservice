pipeline{
	agent any
	environment { 
		 dockerHome = tool 'myDocker'
		 mavenHome = tool 'myMaven'
		 PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
		}
	stages{
		stage('Build'){
			steps{
				//bash 'node --version'
				//bash 'mvn --version'
				echo 'Build in another version'
				
			}
		}
		stage('Test'){
			steps{
				echo 'Test'
			}
		}
		stage('Integration test'){
			steps{
				echo 'Integration test'		
			}
		}
	}
	post {
		always { 
			echo 'Im awesome..I run always..'
		}
		success {
			echo 'I run when you are successful'
		}
		failure {
			echo 'I run when you are failed'
		}

	}
}
