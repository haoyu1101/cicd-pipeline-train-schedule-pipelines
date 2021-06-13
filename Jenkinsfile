pipeline {
/*retrict which agent to run on*/
  agent any
/*Define the stage*/
  stages {
/*stage name*/
    stage ('Build') {
/*Define the steps*/
      steps {
        /*print text to the console, execute a command line - run the build locally with turn off the gradle daemon(background process to speedup the build)*/
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
