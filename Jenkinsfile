pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=aliawebapp -Dsonar.organization=aliawebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=39fdf68c3ca22b7572068d7bf5f862a4c22e9649'
			}
        } 
  }
}
