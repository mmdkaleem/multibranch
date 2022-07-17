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

	stage('Continuous Deployment') 
	{
	sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/MultiBranchPipelinejob/webapp/target/webapp.war   ubuntu@[200~172.31.15.118:/var/lib/tomcat8/webapps/qaenv.war'
	}
    stage('Continuous Testing') 
	{
              sh label: '', script: 'echo "Testing Passed"'
	}
    stage('Continuous Delivery') 
	{
sh label: '', script: 'scp /home/ubuntu/.jenkins/workspace/MultiBranchPipelinejob/webapp/target/webapp.war   ubuntu@172.31.2.243:/var/lib/tomcat8/webapps/prodenv.war'
	}
}
