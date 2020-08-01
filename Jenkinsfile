pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'ls'
        sh 'mvn --version'
        echo '..... Build Phase Started :: Compiling Source Code :: .....'
        dir(path: 'java_web_code') {
          sh 'mvn install'
        }

      }
    }

  }
}
