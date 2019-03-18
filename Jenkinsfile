pipeline {
  agent none
  stages {
    stage('Run Tests') {
      agent {
        label 'macos'
      }
      steps {
        sh 'brew install rust'
        sh 'cargo build'
        sh 'cargo test'
      }
    }
  }
}
