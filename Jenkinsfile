pipeline{
	agent any
	environment{
		staging_server="44.211.124.172"
	}
		stages{
			stage('Deploy to remote'){
				steps{
					sh 'scp -r ${WORKSPACE}/* root@${staging_server}:/var/www/html/leavesystem/'
				}
			
			}
		}


}
