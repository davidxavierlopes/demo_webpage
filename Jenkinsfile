pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing Docker Image'
          }
        }

        stage('Test 2') {
          steps {
            echo 'Testing HTML Syntax'
          }
        }

      }
    }

    stage('Staging') {
      steps {
        echo 'Dev Env'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }

  }
}