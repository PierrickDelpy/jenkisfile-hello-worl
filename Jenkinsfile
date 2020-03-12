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
                publishHTML([
                        allowMissing: true,
                        alwaysLinkToLastBuild: true,
                        keepAll: true,
                        reportDir: "/",
                        reportFiles: 'artifact.txt',
                        reportName: 'Artifact',
                        reportTitles: 'Artifacts'
                    ])
            }
        }
     }
}
