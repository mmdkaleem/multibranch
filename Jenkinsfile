node('built-in') 
{
    stage('Continuous Download_master') 
	{
    git 'https://github.com/mmdkaleem/multibranch.git'
	}
    stage('Continuous Build_master') 
	{
    sh label: '', script: 'mvn package'
	}
}
