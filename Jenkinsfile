pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build done'
      }
    }

    stage('Dev') {
      parallel {
        stage('Dev') {
          steps {
            echo 'dev done'
          }
        }

        stage('QA') {
          steps {
            echo 'deploy to QA : done'
          }
        }

      }
    }

    stage('Prod') {
      steps {
        echo 'Deployed to production'
      }
    }

  }
}