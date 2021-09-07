pipeline {
  agent any
parameters {
	    choice: (name: 'VERSION' 'choices, [1,2,3]', description: '')
	    booleanParam:(paramName: 'executeTest', defaultvaue:'True', description:'')
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
    stage('Deploy') 
	  when {
		  expression {
			  param.executeTest}
      steps {
      echo 'Deploy de app'
      } 
		}
  }
  
}
  node {
    // Groovy script
  }
