pipeline {
  agent any
  tools { 
        maven 'maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=vulnapp -Dsonar.organization=vulnapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=8cbf9e1b947cf3e98ff30cf039520e2ff95fccb9'
			}
        } 
  }
}
