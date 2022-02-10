pipeline {
  agent any
  stages {
    stage('Docker Build') {
steps {
         script {
          switch(GIT_BRANCH) {
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
