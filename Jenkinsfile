pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build'
        sh './gradlew build --no-daemon'
        archiveArtifacts 'dist/trainsSchedule.zip'
      }
    }
  }
}
