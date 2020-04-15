pipeline
{
 agent any
 stages{
 
 stage('Build application'){
 steps{
 bat 'mvn clean install'
 }
 }
 
 stage('Deploy application to CloudHub'){
  steps{
 bat 'mvn package deploy -DmuleDeploy'
 }
 }
 
 stage('Perfrom Regression Testing'){
  steps{
 bat 'newman run M:\\Akhilesh\\Cognizant\\Study\\Mule4\\Newman_Postman_collection\\World_TimeZone.postman_collection.json --disable-unicode'
 }
 }
 
 }
 
}
