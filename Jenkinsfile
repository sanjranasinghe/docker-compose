pipeline {
    agent any
    stages {
      
     
        stage("Test") {
            when {
                not {
                    branch "test"
                }
            }
            steps {
                echo "Test stage."
            }
        }
    }
}

