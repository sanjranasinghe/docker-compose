properties([parameters([gitParameter(branch: '', branchFilter: 'origin/(.*)', defaultValue: 'origin/*', name: 'BRANCH', quickFilterEnabled: false, selectedValue: 'NONE', sortMode: 'NONE', tagFilter: '*', type: 'PT_BRANCH')])])
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

