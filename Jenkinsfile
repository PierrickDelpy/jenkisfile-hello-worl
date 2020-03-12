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
           archiveArtifacts 'artifact.txt' 
        }
     }
}
