/* groovylint-disable-next-line CompileStatic */
pipeline {
    agent any
    stages {
        stage('Unit Test') {
          steps {
            sh 'npm install'
            sh 'ng test  --watch=false --browsers=ChromeHeadlessNoSandbox && echo "Unit Test Passed"'
          }
        }

        stage('Build') {
          steps {
            sh 'ng build'
          }
        }
    }
}
