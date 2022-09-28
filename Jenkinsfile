pipeline{
	agent {
		label {
			label ('built-in')
		}
	}
	stages {
		stage ('master') {
			steps {
				echo "this is master"
			}
		}
		stage ('node-1') {
			agent {
				label {
					label ('slave2')
				}
			}
			steps {
				 echo "hello"
			}
		}

	}
}
