
CODE_CHANGES = getGitChanges()
pipeline {
  agent any
  stages {
      stage('Build') {
          when {
              expresion {
                  BRANCH_NAME == 'dev' && CODE_CHANGES == true       
              }
           }       
           steps {
               echo 'Build de app'
	         }
	    }		
       stage('Install') {
            steps {
                echo 'Install de app'
            }
      }  
         stage('Deploy') {
             when {
                expresion {
                    BRANCHE_NAME == 'dev'
                }
             }
            steps {
                echo 'Deploy de app'
            } 
		      }
  }
  
}
  node {
    // Groovy script
  }
