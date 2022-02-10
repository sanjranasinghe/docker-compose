pipeline {
  agent any
  stages {
    stage('Docker Build') {
      when {
        branch 'main'
      }
      steps {
            echo "hi"
      }
    }

    stage('Docker Push') {
      when {
        branch 'test'
      }
      steps {
        echo "test"
    }
  }
}
}
