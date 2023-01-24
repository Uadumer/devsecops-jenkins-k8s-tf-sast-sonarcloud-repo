pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp1 -Dsonar.organization=asgbuggywebapp1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=8b06958fab78ea34e94bfd18037a442898fb50e2'
                 } 
         }
     }
}
