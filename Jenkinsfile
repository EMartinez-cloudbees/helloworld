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
      agent any
      steps {
        echo 'Buzz unit testing'
      }
    }

    stage('BuzzRegressionTest') {
      agent any
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
pipeline {
  agent none
  stages {
      stage('Stage one') {
      agent any  
      steps {
        echo 'From a different pipeline'
      }
    }
  }
  options {
    timeout(time: 1, unit: 'MINUTES')
  }
}  
