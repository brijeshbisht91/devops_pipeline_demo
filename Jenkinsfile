pipeline {
  agent any
  environment{
//    PATH ="/Users/brijeshbisht/.jenkins/workspace/devops_pipeline"
  }
  stages {
    stage('build') {
      steps {
     //   sh '${PATH}/java_web_code'
        
        dir("${env.WORKSPACE}/java_web_code"){
    sh "pwd"
}
        sh 'ls'
        sh 'mvn --version'
        sh 'mvn install'
        echo '..... Build Phase Started :: Compiling Source Code :: .....'
      }
    }

  }
}
