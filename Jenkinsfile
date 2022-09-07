pipeline {
  agent any
  stages {
    stage('compile-app') {
      steps {
        echo 'this is the compile job'
        sh 'maven compile'
      }
    }

    stage('test-app') {
      steps {
        echo 'this is the test job'
        sh 'mvn test'
      }
    }

    stage('package-app') {
      steps {
        echo 'this is the package job'
        sh 'mvn package'
      }
    }

   
  }
  tools {
    maven 'maven'
  }
  post {
    always {
      echo 'Hey, this is my firts pipeline as code....'
    }

  }
}
