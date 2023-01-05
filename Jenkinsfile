pipeline{
	agent any
	environment{
		staging_server="44.211.124.172"
	}
		stages{
			stage('Deploy to remote'){
				steps{
					sh 'scp -r ${ec2-user@ip-172-31-95-46}/* root@${staging_server}:/var/www/html/leavesystem/'
				}
			
			}
		}


}
