pipeline{
	agent{
		label{
			label'built-in'
			customWorkspace'/mnt/projectdocker'
		}
	}
	stages{
		stage('deploy sample.war'){
			steps{
				sh 'docker-compose down'
				sh 'docker-compose up -d'
			}
		}
	}
}
