pipeline {
  agent any
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
            bat 'java -jar "C:/Program Files (x86)/Jenkins/workspace/Task1/target/Micro_Academy-1.0-SNAPSHOT.jar"'
         }
      }
   }
}
