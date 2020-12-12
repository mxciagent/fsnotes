pipeline {
  agent any
  stages {
    stage('Checkout Branch') {
      steps {
        git(url: 'https://github.com/mxciagent/fsnotes.git', branch: 'master', poll: true, credentialsId: 'mxciagent')
      }
    }

    stage('Install Pods') {
      steps {
        sh 'pod install'
      }
    }

  }
}