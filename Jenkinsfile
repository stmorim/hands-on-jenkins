pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building...'
      }
    }

    stage('Test Firefox') {
      parallel {
        stage('Test Firefox') {
          steps {
            sh 'echo "firefox test"'
          }
        }

        stage('Test Chrome') {
          steps {
            sh 'echo "chrome test"'
          }
        }

        stage('Test Edge') {
          steps {
            sh 'echo "edge test"'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

  }
}