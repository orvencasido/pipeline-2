pipeline{
	agent any 

	environment{
		NAME="Orbs"
		LAST_NAME="Casido"
		secret=credentials('SECRET_NAME')
	}

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
		stage('Name'){
			steps{
				sh '''
					echo "Hello! $NAME $LAST_NAME"
				'''
			}
		}
		stage('Secret'){
			steps{
				sh '''

					echo "$secret"
				'''
			}
		}
	}
}
