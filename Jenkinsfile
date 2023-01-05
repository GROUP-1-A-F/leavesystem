pipeline{
	agent any
	environment{
		server_name="44.211.124.172"
	}
		stages{
			stage('Deploy to remote'){
				steps{
					sh 'scp -r ${WORKSPACE}/* root@${server_server}:/var/www/html/leavesystem/'
				}
			
			}
		}


}
