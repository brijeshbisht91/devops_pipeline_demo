pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''cd java_web_code
mvn install
'''
        echo '..... Build Phase Started :: Compiling Source Code :: .....'
      }
    }

  }
}