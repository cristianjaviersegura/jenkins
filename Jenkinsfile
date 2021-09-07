pipeline {
  agent any

  stages {
    stage('Build') {
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
	    expression {
			  params.executeTest}
	  }
      steps {
      echo 'Deploy de app'
      } 
		}
}
