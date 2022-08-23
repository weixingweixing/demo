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
