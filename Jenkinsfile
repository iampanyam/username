pipeline {
  agent {
        label 'master'
            }
  stages {
    stage('build user') {
      steps {
        wrap([$class: 'BuildUser']) {
          sh 'echo "${BUILD_USER}"'
        }
      }
    }
  }
}
