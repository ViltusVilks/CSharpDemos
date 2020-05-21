pipeline {
  agent any
  stages {
    stage('Step #1') {
      parallel {
        stage('Step #1') {
          steps {
            sh 'echo A'
          }
        }

        stage('Step 1.2') {
          steps {
            sh 'ech B'
          }
        }

        stage('step 1.3') {
          steps {
            sh 'echo C'
          }
        }

      }
    }

    stage('Ste 2.0') {
      steps {
        sh 'echo 2.1'
      }
    }

  }
}