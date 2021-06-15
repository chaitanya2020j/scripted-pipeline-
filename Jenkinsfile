pipeline {
  agent any
  stages {
    stages ('clone repo and clean it') {
      steps{
        sh "rm-rf my-app"
        sh "git clone https://github.com/chaitanya2020j/scrited-pipeline-"
        sh "mvn clean -f scripted"
      }
    }
    stage('--test--') {
      steps{
        sh "mvn test"
      }
    }
    stage('--package--') {
      steps{
        sh "mvn package"
      }
    }
  }
}
