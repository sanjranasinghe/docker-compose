pipeline {
    agent any
    stages {
      
      stage('scm'){
     steps{
        
        git url: 'https://github.com/sanjranasinghe/docker-compose.git'
   
     
     }
        stage("Test") {
            when {
                not {
                    branch "master"
                }
            }
            steps {
                echo "Test stage."
            }
        }
    }
}
}
