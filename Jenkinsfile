@Library('shared-library-ci@master')_

pipeline{
	agent any
//    	tools { 
//        	maven 'maven-3.6.1' 
//	 }
	stages{
		stage('scm checkout'){
			steps{
				script {
					shoppingcart-cleanws
				}
			}
		}
	}
}
