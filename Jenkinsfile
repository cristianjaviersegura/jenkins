pipeline {
  agent any
  environment {
      NEW_VERSION = '1.3.0'
  }
  stages {
      stage("Build") {
           steps {
               echo 'Build de app'
               echo "buinding the app ${NEW_VERSION}"
	         }
	    }		
       stage("Install") {
            steps {
                echo 'Install de app'
            }
      }  
         stage("Deploy") {
            steps {
                echo 'Deploy de app'
            } 
		      }
  }
  
}
  node {
    // Groovy script
  }
