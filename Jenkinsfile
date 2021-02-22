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
                                        sh 'ls -l'
                                        sh 'terraform init'
					sh 'terraform apply -auto-approve'
				}
			}
		}
	}
}
