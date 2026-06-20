pipeline {
  agent any
  tools { 
        maven 'Maven_3.8.4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh "mvn clean verify sonar:sonar -Dsonar.projectKey=freyapvasbuggywebapp -Dsonar.organization=Matr33shka -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=99e831abb97743506749da2eaff956805abbc35e"
			}
        } 
  }
}
