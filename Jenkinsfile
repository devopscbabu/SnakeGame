pipeline {
    agent any
    tools {
        maven 'M2_HOME'
    }
stages {
    stage('Checkout from Github') {
      steps {
         git branch: 'master', url: 'https://github.com/devopscbabu/SnakeGame.git'
            }
    }
  stage('Build using maven') {
      steps {
         sh 'mvn clean package'
             }
    }
  }
}
