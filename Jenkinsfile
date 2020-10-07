pipeline {
  agent any
  stages {
    stage('hello') {
      steps {
        echo 'hellow2'
      }
    }
    stage('deproy') {
      when {
        branch 'master'
      }
      steps {
        echo 'deprooooooooooy!'
      }
    }
  }
}