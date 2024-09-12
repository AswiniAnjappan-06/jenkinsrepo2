pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build done successfully'
      }
    }

    stage('DEV') {
      parallel {
        stage('DEV') {
          steps {
            echo 'Deployment successful'
          }
        }

        stage('QA') {
          steps {
            echo 'QA successful'
          }
        }

      }
    }

    stage('Prod') {
      steps {
        echo 'Production successul'
      }
    }

  }
}