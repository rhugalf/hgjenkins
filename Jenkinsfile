pipeline {
	agent any
	environment{
		dockerHome= tool 'myDocker'
		mavenHome = tool 'myMaven'
		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
	}
	stages {
		stage('CheckOut'){
			steps{

				echo "Build"
				echo "$PATH"
				echo "build number - $env.BUILD_NUMBER"
				echo "$env.BUILD_ID"
				echo "$env.JOB_NAME"
				echo "$env.BUILD_TAG"
			}
		}
		stage('Compile'){
			steps{
				sh 'mvn clean compile'
			}
		}
		stage('Test'){
			steps{
				echo "Teste"
				sh 'mvn test'
			}
		}
		stage('IT'){
			steps{
				echo "IT TEEEESTY"
				sh 'uname -a'
				sh 'mvn failsafe:integration-test failsafe:verify'
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