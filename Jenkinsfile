pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=equiwbuggywebapp -Dsonar.organization=equiwbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=fcfe33f5169a4afb95b253406ae55d5f54f8b116'
			}
        } 
  }
}
