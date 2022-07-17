node('built-in') 
{
    stage('Continuous Download_loans') 
	{
    git 'https://github.com/mmdkaleem/multibranch.git'
	}
    stage('Continuous Build_Loans') 
	{
    sh label: '', script: 'mvn package'
	}
}
