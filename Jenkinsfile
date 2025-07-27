pipeline
{
	agent any
	stages
	{
		stage('Code Checkout')
		{
			steps
			{
			  git branch: 'main', 	
				git 'https://github.com/VaibhavBist/july12igp.git'
			}
		}
		
		stage('Code Compile')
		{
			steps
			{
				sh 'mvn compile'
			}
		}

		stage('Unit Test')
		{
			steps
			{
				sh 'mvn test'
			}
		}

		stage('Code packaging')
		{
			steps
			{
				sh 'mvn package'
			}
		}
   }
}