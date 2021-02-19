pipeline {
  agent any
  
  stages {
    stage('Setup') {
      steps {
        git url: 'https://github.com/CristhianFG/hello-spring_maven.git', branch:'main'
      }
    }
    stage('Build') {
      steps {
        withMaven {
          sh 'mvn package'
        }
      }
    }
  }
}
