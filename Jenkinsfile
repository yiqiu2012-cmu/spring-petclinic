pipeline {
  agent any
  stages {
    stage('Scan') {
      steps {
        sh ''' sonar-scanner \\
  -Dsonar.projectKey=sonarqube-yiqiu \\
  -Dsonar.sources=. \\
  -Dsonar.exclusions=vendor/**,resources/**,**/*.java \\
  -Dsonar.host.url=http://localhost:9000 \\
  -Dsonar.login=d64ca9e692bb9f969c455a90f427aa3379ae8172'''
      }
    }

  }
}