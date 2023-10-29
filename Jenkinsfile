pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=dsobuggyapp_dsobuggyapp -Dsonar.organization=dsobuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e95c370c05342d00c93c860ab0939a3b29ab1197'
			}
        } 
  }
}
