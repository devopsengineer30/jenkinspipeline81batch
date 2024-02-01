pipeline {
  agent any
  stages {
    stage('plan') {
      steps {
        echo 'Plan for pipeline'
      }
    }

    stage('Code') {
      steps {
        echo 'Prepare code for pipeline'
      }
    }

    stage('Build') {
      steps {
        echo 'Build code for pipeline'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Test Code for pipeline'
          }
        }

        stage('Release') {
          steps {
            echo 'Release code for pipeline'
          }
        }

        stage('Deploy') {
          steps {
            echo 'Deploy code for pipeline'
          }
        }

        stage('Operate') {
          steps {
            echo 'Operate Code for Pipeline'
          }
        }

      }
    }

  }
}