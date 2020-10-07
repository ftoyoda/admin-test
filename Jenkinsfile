pipeline {
  agent any
  stages {
    stage('test') {
      when {
        anyOf {
          changeRequest target: 'master'
          branch 'master'
        }
      }
      steps {
        echo 'testeeeeeee!'
      }
    }
    stage('deproy') {
      when {
        branch 'master'
        not {
          changeRequest target: 'master'
        }
      }
      steps {
        echo 'deprooooooooooy!'
      }
    }
  }
}


/*
  -- only if push to master - and no pull request
  when {
    branch 'master'
    not {
      changeRequest target: 'master'
    }
  }

  -- only if pull request and if it is to master
  when {
    changeRequest target: 'master'
  }
*/