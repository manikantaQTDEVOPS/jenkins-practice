pipeline {
      // agent is allocated with the label jdk17
     agent { label 'JDK17'}
     options {
      // cancel the build if there is any problem after 10 minutes
      timeout(time: 10, unit: 'MINUTES')
 }

    parameters {
       string( name: 'PERSON' , defaultVlaue: 'MANIKANTA')
    }
     stages {
      stage('Example') {
            steps {
                  echo 'Hello-World'
            }
      }
     } 

     //post section in the pipeline
     post {
      success {
            echo 'pipeline success'
            // when the pipeline success print the success msg    
      }
      failure {
            echo 'pipeline failure'
            // when the pipeline failure print the failre msg
      }
      // always {
      //       echo 'success or failure'
      //       // when the pipeline success or failure print the always msg
      // }
     }
}
