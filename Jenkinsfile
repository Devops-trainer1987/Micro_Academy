pipeline {
   agent {label 'Win_Server'}

   stages {
      stage('Compile') {
         steps {
            bat 'mvn compile'
         }
      }
      stage('Test') {
         steps {
            bat 'mvn test'
         }
      }
      stage('Package') {
         steps {
            bat 'mvn package'
         }
      }
      stage('Execute') {
         steps {
            bat 'java -jar "c:/MVN/workspace/Micro_Pipeline_Slave/target/Micro_Academy-1.0-SNAPSHOT.jar"'
         }
      }
   }
}
