pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        echo 'Build Stage Successful'
      }
    }
    stage('Test'){
      steps{
        echo 'Test Stage Successful'
      }
    }
  }
  stage('Test'){
    steps{
      echo 'Test Stage Successful'
    }
   }
  }
  post{
    failure{
      echo 'Pipeline failed'
    }
  }
}
