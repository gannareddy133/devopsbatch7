pipeline {
  agent any
  stages {
    stage('dev ') {
      steps {
        echo 'This is dev stage'
      }
    }

    stage('build') {
      steps {
        echo 'This is build stage'
      }
    }

    stage('test') {
      steps {
        echo 'This is test stage'
      }
    }

    stage('uat') {
      parallel {
        stage('uat') {
          steps {
            echo 'This is uat stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'This is deploy stage'
          }
        }

        stage('operation') {
          steps {
            echo 'This is operation stage'
          }
        }

      }
    }

  }
}