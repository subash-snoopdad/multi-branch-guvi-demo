pipeline {
  agent any

  stages {
    stage('Environment Decision') {
      steps {
        script {
          if(env.BRANCH_NAME == "main") {
            echo "Production Branch"
          }
          else if(env.BRANCH_NAME == "develop") {
            echo "QA Branch"
          } else {
            echo " Feature Branch"
          }
        }
      }
    }
  }
}
