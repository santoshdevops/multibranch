	node {
		stage('Clean') {
		 sh 'mvn clean'
			 }

		 stage('Build') 
		 {
			if (env.BRANCH_NAME == 'master') 
			{
				echo 'I only execute on the master branch'
				git url: 'https://github.com/santoshdevops/multibranch.git'
				sh "/bin/mvn clean"
				sh "/bin/mvn package -DskipTests"
				
			} else 
			{
				echo 'I execute elsewhere'
			}
		}	
		
		
		
		stage('deploy') 
		{
			if (env.BRANCH_NAME == 'master') 
			{
				echo 'I only execute on the master branch'
				git url: 'https://github.com/santoshdevops/multibranch.git'
				sh "/bin/mvn package -DskipTests"
				
			} else 
			{
				echo 'I execute elsewhere'
			}
		
			
		}
		
		
		}
		
		
			
		
		
		
		
		
