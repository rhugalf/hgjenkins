pipeline {
	agent any
	stages {
		stage('Build'){
			steps{
				echo "Build"
			}
		}
		stage('Test'){
			steps{
				echo "Teste"
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
		finally{
			echo "a chingar as u madre"
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