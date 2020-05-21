pipeline {
  agent any
  stages {
    stage('Step #1') {
      parallel {
        stage('Step #1') {
          steps {
            sh '''sleep 25
echo A
seep 21
echo A finished'''
          }
        }

        stage('Step 1.2') {
          steps {
            sh '''sleep 23
echo B
seep 21
echo B finished'''
          }
        }

        stage('step 1.3') {
          steps {
            sh '''sleep 23
echo C
seep 21
echo C finished'''
          }
        }

        stage('error') {
          steps {
            sh '''sleep 21
echo D
seep 21
echo D finished'''
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