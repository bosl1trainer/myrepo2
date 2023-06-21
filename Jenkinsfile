pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          agent any
          steps {
            sh 'echo "step1"'
            sh 'echo "step2"'
          }
        }

        stage('Stage2') {
          agent any
          steps {
            echo 'Step3'
            echo 'step4'
          }
        }

      }
    }

    stage('Stage3') {
      agent any
      steps {
        sh 'echo "step1 of stage3"'
      }
    }

  }
}