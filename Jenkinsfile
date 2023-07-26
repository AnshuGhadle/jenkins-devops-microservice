pipeline {
    agent { docker { image "maven"}}
        stages {
            stage('Build') {
                steps{
					sh "mvn --version"
                    echo "Build"
                }
			}
			  stage('Test') {
                steps{
                    echo "Test"
                }
			}
			  stage('Integration Test') {
                steps{
                    echo "Integration Test"
                }
			}
		}
		post{
				always{
					echo "Iam awesome. I always run"
				}
				success{
					echo "I run when you are successful"
				}
				failure{
					echo "I run when you fail"
				}
		}

}
               
               
                
