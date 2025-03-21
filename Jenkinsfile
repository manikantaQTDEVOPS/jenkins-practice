pipeline {
      // agent is allocated with the label jdk17
     agent { label 'JDK17'}
     options {
      // cancel the build if there is any problem after 10 minutes
      timeout(time: 10, unit: 'MINUTES')
 }
  //added the pipeline owner in the parameters block

    parameters {
       string( name: 'PERSON' , defaultValue: 'MANIKANTA')
    }
     stages {
      stage('Example') {
            steps {
                  echo 'Hello-World'
            }
      }
      stage( 'params stage') {
            steps {
                  echo "Hello ${params.PERSON}"
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
      
     }
}
