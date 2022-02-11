pipeline {
  agent any
  stages {
    
     stage("git"){
            
            steps{
                
                git branch: 'main', url: 'https://github.com/sanjranasinghe/docker-compose.git'

            }
            
            }
    
    
    stage('Docker Build') {
steps {
         script {
          switch(BRANCH) {
            case "main": 
              echo 'main sanjaya1'
              break
            case "test": 
              echo 'test2'
              break
          }
        }
      }
    }

    
}
}
