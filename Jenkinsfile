pipeline {
  agent any
  stages {
    stage('version') {
      steps {
        sh 'jbang version'
      }
    }
    stage('full path') {
      steps {
        sh 'jbang run scripts/greeting.java'
      }
    }
  }
}