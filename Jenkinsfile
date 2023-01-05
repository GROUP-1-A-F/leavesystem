pipeline{
	agent any
	environment{
		server_name="44.211.124.172"
	}
		stages{
			stage('Deploy to remote'){
				steps{
					sh 'scp -r ${WORKSPACE}/* root@44.211.124.172:/var/www/html/leavesystem/'
				}
			
			}
		}


}
