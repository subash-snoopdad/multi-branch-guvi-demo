pipeline {
  agent any

  stages {
    stage('Branch Information') {
      steps {
        echo "Current Branch = ${env.BRANCH_NAME}"
      }
    }

    stage('System Information') {
      steps {
        sh '''
        hostname
        date
        pwd
        '''
      }
    }
  }
}
