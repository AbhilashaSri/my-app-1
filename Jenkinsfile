node
	{
	    stage('git checkout')
	    {
	        git 'https://github.com/mohankrishna23/hello-world.git'
	    }
	   stage('files present at git')
	   {
	       sh "ls -lrt"
	   }
	   stage('build and compile')
	   {
           def mvnHome = tool name: 'Maven', type: 'maven'   //returns maven home directory
	   sh "${mvnHome}/bin/mvn package"
	   }
	   stage('email notification')
	   {
	 emailext body: 'test email', subject: 'test email', to: 'abhilasha.srivastava@kpn.com'
	   }
	}
