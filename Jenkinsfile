pipeline {
  agent any
  stages {
    stage('t1') {
      steps {
        sleep 200
      }
    }
    stage('t12') {
      steps {
        sleep 200
      }
    }
    stage('') {
      steps {
        git 'https://github.com/8562727/disconf.git'
        sshPublisher(alwaysPublishFromMaster: true, continueOnError: true)
      }
    }
  }
}