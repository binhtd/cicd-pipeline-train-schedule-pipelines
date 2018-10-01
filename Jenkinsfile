pipeline {
  agent any
  
  stages {
    stage("Build") {
      echo "Running build"
      sh "../gradlew build --no-daemon"
      archiveArtifacts artifacts: "dist/trainSchedule.zip"
    }
  }
}
