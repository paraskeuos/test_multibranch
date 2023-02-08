pipeline {
  agent {
    node {
      label 'linux'
    }
  }

  stages {
    stage('main') {
      when {
        branch 'main'
      }

      steps {
        echo 'main'
      }
    }

    stage('dev') {
      when {
        branch 'dev'
      }

      steps {
        echo 'dev'
      }
    }
  }
}

