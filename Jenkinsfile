pipeline {
  agent any
  statges {
     stage build ('Build') {
       steps {
          echo 'Running build automation...'
          sh './gradlew build --no-daemon'
          archiveArtifacts artifacts: 'dist/trainSchedule.zip'
       }
    }
  }
}
