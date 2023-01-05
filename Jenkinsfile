pipeline{
	agent any
	environment{
		staging_server="172.31.95.46"
	}
		stages{
			stage('Deploy to remote'){
				steps{
					sh 'scp -r ${WORKSPACE}/* root@$staging_server}:/var/www/html/leavesystem/'
				}
			
			}
		}


}
