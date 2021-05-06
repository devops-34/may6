pipeline {
    agent any 
  stages {
  
  stage ('common') {
   sh echo "stage1"

    stage ('Two') {
      when {
                expression { params.env == 'UI'}
            }
            steps {
              sh  echo "Hello, Test"
            }
    }
    stage ('UAT') {
      when {
                expression { params.env == 'UAT'}
            }
            steps {
               sh  echo "Hello, UAT"
            }
    }
   
  }
}
