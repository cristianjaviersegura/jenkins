pipeline {
  agent any
parameters {stringname: (name: 'VERSION,defaultvalue: '',description: 'version to deploy')
	    choice: (name:  'choices, [1,2,3]', description: ')
	    booleanParam:(paramName: 'executeTest', defaulvaue:'True', description:'')
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
