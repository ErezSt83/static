pipeline {
	agent any 
	stages {
		stage('Build') {
			steps  {
				withAWS(region:'us-west-2', credentials: 'Jenkins') {
					s3Upload(file:'index.html', bucket:'myudacityprojectjenkins', path:'/index.html')				
				}
			}
		}
	}
}