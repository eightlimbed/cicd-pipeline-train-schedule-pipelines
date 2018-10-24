# Defines the CI/CD Pipeline

pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Running build automation (from: Jenkinsfile)'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
