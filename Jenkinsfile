/* groovylint-disable-next-line CompileStatic */
pipeline {
    agent any
    stages {
        stage('Unit Test') {
          steps {
            sh 'npm install'
            sh 'npm test'
          }
        }

        stage('Build') {
          steps {
            sh 'ng build --prod'
          }
        }
    }
}
