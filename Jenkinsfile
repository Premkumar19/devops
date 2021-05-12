  pipeline{
	agent any
		stages{
			stage('one'){
				steps{
					echo "This is POC session"
			}
		}
			stage('two'){
				steps{
					input('do you want to proceed?')
			}
		}
			stage('three'){
				when{
					not{
						branch "master"
				}
			}
				steps{
					echo "Hello team"
			}
		}
			stage('Unit test'){
				steps{
					echo "running unit test"
			}

		}
	}
}
