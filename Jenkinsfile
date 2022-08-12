pipelines {
  agent any
  stages {
    stage ('build') {
      steps {
        echo "Running build automation" 
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
