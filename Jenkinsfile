pipeline {
  agent any
  stages {
    stage('Step #1') {
      parallel {
        stage('Step #1') {
          steps {
            slackSend(message: 'zzz 1', attachments: '[]', blocks: '[]')
          }
        }

        stage('Step 1.2') {
          steps {
            waitUntil(initialRecurrencePeriod: 5) {
              sh 'echo A'
            }

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