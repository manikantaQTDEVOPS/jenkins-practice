pipeline {
  // agent is allocated in the stage      
      agent none
      stages {
            stage('Example') {
                  agent any 
                   options {
                        // timeout counter starts before agent is allocated
                        timeout(time: 10, unit: 'SECONDS')
                   }
                   steps {
                        echo 'Hello-Worid'
                   }
                  

                  }
            }
      }
