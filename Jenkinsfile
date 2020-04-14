pipeline {
  agent none
  stages {
    stage('BuzzBuild') {
      agent any
      steps {
        echo 'buzz building'
      }
    }

    stage('BuzzUnitTest') {
      steps {
        echo 'Buzz unit testing'
      }
    }

    stage('BuzzRegressionTest') {
      steps {
        echo 'Buzz regression test'
        echo 'xml to Junit'
        echo 'send email'
      }
    }

  }
  options {
    timeout(time: 1, unit: 'MINUTES')
  }
}