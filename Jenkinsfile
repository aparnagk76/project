pipeline {
  agent { label 'mynode' }
  stages {
    stage('Compile') {
      steps {
        sh './gradlew clean compileJava'
      }
    }
    stage('Test') {
      steps {
        sh './gradlew test'
      }
    }
    stage('Package') {
        steps {
            sh 'echo package'
        }
    }
    stage('Deploy') {
        steps {
            sh 'echo deploy'
        }
    }
  }
}
