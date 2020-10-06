pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Run build automation'
        sh './gradlew build --no-daemon'
        archieveArtifacts artifacts: 'dist/trainSchedule.zip'
        
      }
    }
  }
}
