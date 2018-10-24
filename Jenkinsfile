
node('master') 
{
  stage('ContinuousDownload-Feature-1') 
  {
    git 'https://github.com/selenium-saikrishna/maven.git'
  } 
  stage('ContinuousBuild-Feature-1') 
  {
    sh 'mvn package'
  } 
  stage('ContinuousDeployment-Feature-1') 
  {
    sh 'scp /home/vagrant/.jenkins/workspace/ScriptedPipeline/webapp/target/webapp.war vagrant@10.0.0.51:/var/lib/tomcat7/webapps/feature.war'
  }
  
  
  
  
  
  
  
  
}
