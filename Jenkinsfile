pipeline {
  agent any
  stages {
    stage('COMMIT') {
      steps {
        echo 'COMMIT THE CODE'
      }
    }

    stage('BUILD') {
      steps {
        echo 'BUILD THE CODE'
      }
    }

    stage('TEST') {
      parallel {
        stage('TEST') {
          steps {
            echo 'TEST THE CODE'
          }
        }

        stage('STAGE') {
          steps {
            echo 'STAGE THE CODE'
          }
        }

        stage('DEPLOY') {
          steps {
            echo 'DEPLOY THE CODE'
          }
        }

        stage('OPERATE') {
          steps {
            echo 'OPERATE THE APP'
          }
        }

      }
    }

  }
}