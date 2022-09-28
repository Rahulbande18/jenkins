pipeline{
	agent {
		label {
			label ('built-in')
		}
	}
	stages {
		stage ('master') {
			steps {
				sh "yum install tree -y"
			}
		}
		stage ('node-1') {
			agent {
				label {
					label ('slave2')
				}
			}
			steps {
				sh "sudo yum install tree -y"
			}
		}

	}
}
