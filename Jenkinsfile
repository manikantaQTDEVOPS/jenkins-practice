pipeline {
      // agent is allocated with the label jdk17
     agent { label 'JDK17'}
     options {
      // cancel the build if there is any problem after 10 minutes
      timeout(time: 10, unit: 'MINUTES')
 }
     stages {
      stage('Example') {
            steps {
                  echo 'Hello-World'
            }
      }
     } 
}
