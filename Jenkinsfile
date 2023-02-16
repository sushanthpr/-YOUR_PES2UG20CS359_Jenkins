pipeline {
    agent any

stages{
  stage('Build') {
    steps{
      sh 'g++ -o PES2UG20CS359 PES2UG20CS359.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './PES2UG20CS359'
    }
  }

  stage('Deploy') {
    steps{
      echo 'DEPLOYMENT SUCCESSFUL'
    }
  }
}
post {
    failure {
        echo 'Pipeline Failed'
    }
  }
}
