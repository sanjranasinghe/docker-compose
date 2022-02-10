pipeline {
  agent any
  stages {
    stage('Docker Build') {
steps {
         script {
          switch(BRANCH) {
            case "main": 
              echo 'main'
              break
            case "test": 
              echo 'test'
              break
          }
        }
      }
    }

    
}
}
