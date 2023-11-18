pipeline { 
  agent any
  options {
      // timeout counter starts after agent is allocated
      timeout(time: 1, unit: 'SECONDS')

  }
  stages {
      stage('Example') {
            steps {
                  echo 'Hello-World'
            }
      }
  }

}