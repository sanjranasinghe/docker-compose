pipeline {
    agent any
    stages {
      
     
        stage("Test") {
            when {
                not {
                    branch "main"
                }
            }
            steps {
                echo "Test stage."
            }
        }
    }
}
