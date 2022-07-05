
pipeline {
  agent any
  stages {
    stage('S1') {
      steps {
        echo 'S1'
      }
    }
    stage('S2') {
      steps {
        echo 'S2'
      }
    }
    stage('Parallel Stages') {
      when {
        branch 'main'
      }
      parallel {
        stage('P1') {
          steps {
            sh 'sleep 120'
          }
        }
        stage('P2') {
          steps {
            sh 'sleep 120'
          }
        }
        stage('P3') {
          steps {
            sh 'sleep 120'
          }
        }
      }
    }
  }
}






