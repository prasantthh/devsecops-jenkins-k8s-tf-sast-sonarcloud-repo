pipeline {
  agent any
  tools { 
        maven 'Maven_3.8.4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=prasantthh -Dsonar.organization=prasantthh -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=8631f57fe0b4ee750a09473ce1a0d0a3099131c1'
			}
        } 
  }
}
