pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        pwd
        ls -lah
        arhiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }  
  }
}
