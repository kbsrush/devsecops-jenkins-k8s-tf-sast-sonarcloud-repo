pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapptest -Dsonar.organization=asgbuggywebapptest -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=d39f7f875db30933ab2e5f0489a067116a718596'
			}
        } 
  }
}
