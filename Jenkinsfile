pipeline {
   agent any

   stages {
      stage('Hello') {
         steps {
            echo 'Hello World'
            sh """ls -l"""
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
