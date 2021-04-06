pipeline {
  agent any
  stages {
    stage('Run') {
      steps {
        sh 'java -jar -Dserver.port=4000 target/*.jar'
      }
    }

  }
}