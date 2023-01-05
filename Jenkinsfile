pipeline{
	agent any
	environment{
		staging_server="44.211.124.172"
	}
		stages{
			stage('Deploy to remote'){
				steps{
				sh '''
					for fileName in `find ${WORKSPACE} -type f -mmin -10 | egrep -v ".git | Jenkinsfile"`
					do
						fil=$(echo ${fileName} | sed 'sed 's/'"${JOB_NAME}"'/ /' | awk{'print $2'})
						scp -r ${WORKSPACE}${fil} root@${staging_server}:/var/www/html/leavesystem${fil}
					done
				'''
				}
			
			}
		}


}
