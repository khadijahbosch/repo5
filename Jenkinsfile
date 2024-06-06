pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Hello Build'
      }
    }

    stage('Unit test') {
      parallel {
        stage('Unit test') {
          steps {
            echo 'Hello  unit'
          }
        }

        stage('Integration test') {
          steps {
            echo 'Hello Integration'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'Hello deploy'
      }
    }

  }
}