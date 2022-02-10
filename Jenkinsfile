properties([parameters([gitParameter(branch: '', branchFilter: 'origin/(.*)', defaultValue: 'origin/*', name: 'BRANCH', quickFilterEnabled: false, selectedValue: 'NONE', sortMode: 'NONE', tagFilter: '*', type: 'PT_BRANCH')])])
pipeline {
  agent any
  stages {
    stage('Docker Build') {
      when {
        branch "main"
      }
      steps {
            echo "hi"
      }
    }

    stage('Docker Push') {
      when {
        branch "test"
      }
      steps {
        echo "test"
    }
  }
}
}
