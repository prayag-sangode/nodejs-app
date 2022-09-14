pipeline {
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git([url: 'https://github.com/prayag-sangode/nodejs-app.git', branch: 'main', credentialsId: 'github-id'])

      }
    }
    stage('Build') {
      steps {
        bat 'npm --version'
        bat 'node --version'
        bat 'npm -i'
        bat 'node app'
      }
    } 
 }
}


