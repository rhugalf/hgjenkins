pipeline {
	agent any
	stages {
		stage('Build'){
			steps{

				echo "Build"
				echo "$PATH"
				echo "build number - $env.BUILD_NUMBER"
				echo "$env.BUILD_ID"
				echo "$env.JOB_NAME"
				echo "$env.BUILD_TAG"
			}
		}
		stage('Test'){
			steps{
				echo "Teste"
				sh 'env'
			}
		}
		stage('IT'){
			steps{
				echo "IT TEEEESTY"
			}
		}	
	}
	post{
		always{
			echo "Furuloooo"
		}
		success{
			echo "jalo esta madre"
		}
		failure{
			echo "VALIO MADREEEE"
		}
	}
}

/**node {
	stage('Build') {
		echo "Build"
	}
	stage('Test') {
		echo "Test"
	}
	stage('Integration Test'){
		echo "TEST IT"
	}
}
*/