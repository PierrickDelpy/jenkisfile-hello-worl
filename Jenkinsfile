pipeline {
   agent any

   stages {
      stage('Hello') {
         steps {
            echo 'Hello World'
         }
      }
   }
   post {
        always {
            script {
                // Publish all Html reports
               archiveArtifacts 'artifact.txt'
            }
        }
     }
}
