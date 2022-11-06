pipeline {
  agent any
  stages {
    stage('log tool version') {
      parallel {
        stage('log tool version') {
          steps {
            sh '''git --version
java -version

'''
          }
        }

        stage('check file') {
          steps {
            fileExists 'pom.xml'
          }
        }

      }
    }

    stage('post build steps') {
      steps {
        writeFile(file: 'status.txt', text: 'hey it worked')
      }
    }

  }
}