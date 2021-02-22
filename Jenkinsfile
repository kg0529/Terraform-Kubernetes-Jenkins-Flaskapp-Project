pipeline{
	agent any
        
	stages{

		stage('check-out'){
			steps{
				checkout scm
			}
		}
		stage('Deploy'){
			steps{
				script {
                                        sh 'terraform init'
					sh 'terraform apply -auto-approve'
				}
			}
		}
	}
}
