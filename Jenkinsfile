pipeline {
  agent any
  stages {
    stage('Static Analysis') {
      steps {
        sh '''sonar-scanner \\
  -Dsonar.projectKey=easy-school \\
  -Dsonar.sources=. \\
  -Dsonar.host.url=http://172.31.80.149:9000 \\
  -Dsonar.login=sqp_fecfcdf34ac789ccda5d7b94c0d2cf9e6a51e6e4'''
      }
    }

  }
}