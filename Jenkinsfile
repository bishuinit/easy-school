pipeline {
  agent {
    node {
      label 'dev'
    }

  }
  stages {
    stage('Static Analysis') {
      steps {
        sh '''sonar-scanner \\
  -Dsonar.projectKey=easy-school \\
  -Dsonar.sources=. \\
  -Dsonar.host.url=http://52.206.217.129:9000 \\
  -Dsonar.login=sqp_e111820a7d7744089b55de30e6d2639800c09646'''
      }
    }

  }
}