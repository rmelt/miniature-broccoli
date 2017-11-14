pipeline {
  agent any
  stages {
    stage('test 1') {
      steps {
        ansiblePlaybook(playbook: 'test', colorized: true, inventory: 'testinv')
        sleep 51
        node(label: 'ansible')
      }
    }
  }
}