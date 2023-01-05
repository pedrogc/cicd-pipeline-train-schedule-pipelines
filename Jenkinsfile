pipeline {
  agent any
  stages {
    stage ('Build') {
      stesp {
        echo 'Running build automation'
        sh './gradlow build --no-daemon'
        archiveArtifects artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
