pipeline {
  agent any
  stages {
    stage('log tool version') {
      steps {
        sh '''git --version
java -version

'''
      }
    }

    stage('Testing') {
      parallel {
        stage('Testing') {
          steps {
            fileExists 'pom.xml'
          }
        }

        stage('Test 2') {
          steps {
            readFile 'pom.xlm'
          }
        }

      }
    }

  }
}