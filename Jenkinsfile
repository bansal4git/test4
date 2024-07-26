pipeline {
  agent any
  stages {
    stage('Pull SCM') {
      steps {
        echo 'SCM Stage Successful'
      }
    }

    stage('Deploy_dev') {
      parallel {
        stage('Deploy_dev') {
          steps {
            echo 'Dev Done'
          }
        }

        stage('Deploy_QA') {
          steps {
            echo 'QA Done'
          }
        }

      }
    }

    stage('Deploy_prod') {
      steps {
        echo 'Prod Done'
      }
    }

  }
}