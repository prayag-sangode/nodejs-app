pipeline {
  agent any
  stages {
    stage('Cloning Git') {
      steps {
        git([url: 'https://github.com/prayag-sangode/java-maven-app.git', branch: 'main', credentialsId: 'github-id'])

      }
    }
    stage('Build') {
      steps {
        sh 'npm -i'
        sh 'node app'
      }
    } 
 }
}


