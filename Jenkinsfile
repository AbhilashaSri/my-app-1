node
	{
	    stage('git checkout')
	    {
	        git 'https://github.com/mohankrishna23/hello-world.git''
	    }
	   stage('files present at git')
	   {
	       sh "ls -lrt"
	   }
	   stage('build and compile')
	   {
	   sh 'mvn package'
	   }
	   stage('email notification')
	   {
	 emailext body: 'test email', subject: 'test email', to: 'abhilasha.srivastava@kpn.com'
	   }
	}
