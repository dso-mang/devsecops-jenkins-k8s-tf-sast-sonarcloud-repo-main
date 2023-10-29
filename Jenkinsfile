pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebapptest -Dsonar.organization=buggywebapptest -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=c0a2e5990a14564bba63d6a03da7fa5c82c3ba24'
			}
        } 
  }
}
