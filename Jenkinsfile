pipeline {
  agent any
  stages {
    stage('Step #1') {
      parallel {
        stage('Step #1') {
          steps {
            sh '''sleep 5
echo A'''
          }
        }

        stage('Step 1.2') {
          steps {
            sh '''sleep 4
echo B'''
          }
        }

        stage('step 1.3') {
          steps {
            sh '''sleep 6
echo C'''
          }
        }

        stage('') {
          steps {
            sh '''sleep 5
echo D'''
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