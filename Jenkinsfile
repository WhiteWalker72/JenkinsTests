pipeline {
  agent {
    docker {
      image 'maven:3.3.9-jdk-8'
      args '-v /root/.m2'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        bat 'mvn -B -DskipTests clean package'
      }
    }
  }
}