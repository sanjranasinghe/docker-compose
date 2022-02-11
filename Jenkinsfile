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
               sshagent(credentials : ["test-servers"]) {
               sh """ssh root@172.16.15.46 << EOF
              mkdir /opt/docker
                     cd /opt/docker
                     git init
                     git pull https://github.com/sanjranasinghe/docker-compose.git
                     ansible-playbook ansible.yml
                     docker-compose up -d
                     exit
                     exit
                     exit
            EOF"""
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
