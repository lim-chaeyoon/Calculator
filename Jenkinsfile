pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        sh './gradlew compileJava'
        sh '''stage("Compile") {
    stpes {
        sh ".gradlew compileJava"
    }
}
'''
        }
      }

      stage('Unit test') {
        steps {
          sh './gradlew test'
        }
      }

    }
  }