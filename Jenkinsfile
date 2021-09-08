pipeline {
  agent any
  parameters {
       choice(name: 'VERSION', choices: ['1.1.0','1.2.0','1.3.0'], description:'')
       booleanParameters(name: 'executeTest', defaultvalue: true, description: '')
  }
  stages {
      stage("Build") {
           steps {
               echo 'Build de app'
	         }
	    }		
       stage("Test") {
            when {
                 expression {
                      params.executeTest
                 }
            }
            steps {
                echo 'test de app'
            }
      }  
         stage("Deploy") {
            steps {
                echo 'Deploy de app'
                echo "deploing version ${params.VERSION}"
            } 
		      }
  }
  
}
  node {
    // Groovy script
  }
