pipeline {
    agent any

stages{
  stage('Build') {
    steps{
      sh 'g++ -o PES2UG20CS351 PES2UG20CS351.cpp'
    }
  }

  stage('Test') {
    steps{
       sh './PES2UG20CS351'
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

