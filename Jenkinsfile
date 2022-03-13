pipeline {
  agent any
  stages {
    stage('1') {
      parallel {
        stage('Up') {
          steps {
            retry(count: 1)
          }
        }

        stage('Down') {
          steps {
            retry(count: 1)
          }
        }

      }
    }

    stage('0') {
      steps {
        retry(count: 1)
      }
    }

  }
}