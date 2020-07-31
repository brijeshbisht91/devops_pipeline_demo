pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'mvn install'
        echo '..... Build Phase Started :: Compiling Source Code :: .....'
      }
    }

  }
}