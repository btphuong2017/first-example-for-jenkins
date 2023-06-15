/* groovylint-disable-next-line CompileStatic */
pipeline {
    agent { docker { image 'node:16.16.0-alpine' } }
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
