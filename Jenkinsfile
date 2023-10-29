pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggywebdso -Dsonar.organization=buggywebdso -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f7668e0603c9ea7d2d6bf44ddf0187ca2b85cac6'
			}
        } 
  }
}
