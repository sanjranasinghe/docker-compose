properties([parameters([gitParameter(branch: '', branchFilter: 'origin/(.*)', defaultValue: 'origin/*', name: 'BRANCH', quickFilterEnabled: false, selectedValue: 'NONE', sortMode: 'NONE', tagFilter: '*', type: 'PT_BRANCH')])])
pipeline {
  agent any
  stages {
    stage('Docker Build') {
      when {
        ${params.BRANCH} 'main'
      }
      steps {
            echo "hi"
      }
    }

    stage('Docker Push') {
      when {
        ${params.BRANCH} 'test'
      }
      steps {
        echo "test"
    }
  }
}
}
