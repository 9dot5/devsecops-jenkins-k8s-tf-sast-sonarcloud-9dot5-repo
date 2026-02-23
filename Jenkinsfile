pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=9dot5BuggyWebApp -Dsonar.organization=9dot5BuggyWebApp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=82e6517cf20f43908925a6315a96303d809e59a3'
			}
        } 
  }
}
