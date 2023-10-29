pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggybaru -Dsonar.organization=buggybaru -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=3b9f6b9abcf79e8aebb7f500282522aed6e93e81'
			}
        } 
  }
}
