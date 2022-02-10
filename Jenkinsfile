properties([parameters([gitParameter(branch: '', branchFilter: '.*', defaultValue: 'origin/*', name: 'BRANCH', quickFilterEnabled: false, selectedValue: 'NONE', sortMode: 'NONE', tagFilter: '*', type: 'PT_BRANCH')])])
pipeline {
    agent any
    stages {
      
     stage('only on master') {
  if (CURRENT_BRANCH == 'test') {
  input {
    echo "Test stage."
  }
}
        }
    }
}
