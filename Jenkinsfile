pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        sh './gradlew compileJava'
        sh '''pipeline {
    agent any
    stages {
    stage("Compile") {
    stpes {
    sh ".gradlew compileJava"
    }
    }
    stage("Unit test") {
    stpes {
    sh "./gradlew test"
    }
}
}
}'''
        }
      }

      stage('Unit test') {
        steps {
          sh './gradlew test'
        }
      }

    }
  }