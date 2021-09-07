pipeline {
  agent any
	parameters {
		stringname: (name 'VERSION,defaultvalue: '',description: ´version to deploy'´
			     )
		choice: (name  'choices, [1,2,3]', description: ')
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
      steps {
      echo 'Deploy de app'
      } 
		}
  }
  
}
  node {
    // Groovy script
  }
