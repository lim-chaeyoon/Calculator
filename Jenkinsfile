pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        sh './gradlew compileJava'
      }
    }

    stage('Unit test') {
      agent any
      steps {
        sh './gradlew test'
        sh './gradlew test'
      }
    }

  }
}