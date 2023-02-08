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
    
    stage('other') {
      when {
        not {
          anyOf {
            branch 'main';
            branch 'dev
          }
        }
      }
      
      steps {
        echo 'some other branch'
      }
    }
  }
}
  
  }
}

