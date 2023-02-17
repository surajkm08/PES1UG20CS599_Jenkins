pipeline{
  agent any
  stages{
    stage('Build'){
      steps{
        sh "g++ -o PES1UG20CS599-1 PES1UG20CS599-1.cpp"
        echo 'Build Stage Successful'
      }
    }
    stage('Test'){
      steps{
         sh 'PES1UG20CS599-1 --test'
        echo 'Test Stage Successful'
      }
    }
    stage('Deploy'){
      steps{
        sh "./PES1UG20CS599-1"
        echo 'Deploy Stage Successful'
      }
    }
  }
  post{
    failure{
      echo 'Pipeline failed'
    }
  }
}
