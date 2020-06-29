pipeline{
	agent any
	stages{
		stage ('Check out'){
			steps{
				echo 'hello'
			}
		}
		stage ('Build'){
			steps{
				echo 'Build'
			}
		}
		stage ('Deploy'){
			steps{
				echo 'Deploy'
			}
		}
		stage ('Test'){
			parallel{
				stage('Unit Test'){
					steps{
						echo "running unit test"
						}
					}
				stage('Integretion Test'){
					steps{
						echo "running integration test"
					}
				}
			}
		}
	}
}