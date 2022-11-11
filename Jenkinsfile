pipeline {
tools{
        jdk 'JAVA_HOME'
		maven 'M2_HOME'
   }
    agent any

    stages {
        stage("checkout") {
            steps {
			git 'https://github.com/LiptiDora/jenkins.git'
               
            }
			}
			
			stage("compile"){
			  steps{
			    sh 'mvn compile'
				}
        
    }
	    
	    stage("package"){
			  steps{
			    sh 'mvn package'
				}
        
    }
}
}
