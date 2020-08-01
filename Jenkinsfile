pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
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

        stage('TEST') {
          steps {
            echo '..... Test Phase Started :: Testing via Automated Scripts :: ......'
            dir(path: 'integration-testing') {
              sh 'mvn clean verify -P integration-test'
            }

          }
        }

      }
    }

  }
}
