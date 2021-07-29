pipeline {
  agent any
  triggers {
    githubPush()
  }
  stages {
    stage('echo') {
      steps {
        echo 'Hello from blue ocean ui'
      }
    }

    stage('buildit') {
      steps {
        bat 'call testscript.bat'
      }
    }

  }
}