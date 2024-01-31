pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=javaprojectreachabilityr -Dsonar.organization=javaprojectreachabilityr -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=794a8e7b24890e868638b1723af97bf2023a37fd'
			}
        } 
  }
}
