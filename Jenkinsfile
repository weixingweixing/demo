pipeline {
  agent {
    node {
      label 'Jenkins_slave_practice'
    }
  }
  stages {
  stage('Init') {
		steps{
			script{
				println "welcome to Nick learn"
			}
		}
	}
  stage('Test'){
               steps{
                      script{
                      container('maven'){
                 sh 'mvn test'
                 println "test 1"
                      }
                }
            }
     }
    stage('maven') {
    		steps{
    			script{
    			container('maven') {
    	          sh 'mvn clean install'	
    			}
    		}
    	}	
    }
  }
}
