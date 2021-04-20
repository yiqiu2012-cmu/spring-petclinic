pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn package'
      }
    }

    stage('deploy') {
      steps {
        ansiblePlaybook(playbook: 'playbook.yaml', inventory: 'inventory.inv')
      }
    }

  }
}