pipeline {

   agent any
   stages {
     stage ('Clean Stage') {
        steps {
	   withMaven (maven: 'MAVEN_HOME'){
	       sh 'mvn clean'
	   }
	}
     }
     stage ('Compile Stage') {
        steps {
           withMaven (maven: 'MAVEN_HOME'){
               sh 'mvn compile'
           }
        }
     }

   }
}
