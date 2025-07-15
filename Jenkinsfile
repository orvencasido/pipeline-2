pipeline{
	agent any 

	stages{
		stage('Build'){
			steps{
				sh '''
					echo "Hello World!"
					ls -lh
					cat README.md
					echo "lets go!"
					echo "letsgo 2"
				'''
			}
		}
		stage ('Create'){
			steps{
				sh '''
					mkdir -p test
				'''
			}
		}
	}
}
