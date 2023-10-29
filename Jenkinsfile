pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=dsobuggywebapp -Dsonar.organization=dsobuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=981646c4c6d5b165b7842840f96d5b03aa39ef5b'
			}
        } 
  }
}
