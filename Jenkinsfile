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
    stage('dir1') {
      steps {
        dir('scripts') {
          sh 'jbang run greeting.java'
        }
      }
    }
    stage('dir2') {
      steps {
        dir('scripts') {
          sh './greeting.java'
        }
      }
    }
    stage('dir3') {
      steps {
        dir('scripts') {
          sh './greeting.java Galaxy'
        }
      }
    }
  }
}