pipeline {
   agent {label 'java'}

  stages {
    stage('Checkout') {
      steps {
        echo 'Checkout'
        checkout scm
      }
    }

    stage('Build') {
      steps {
        sh 'mvn clean package'
      }
    }
     
     stage('Test') {
      steps {
        echo 'Test'   
        sh 'mvn test'
      }
    }
  }

}
