pipeline {
    agent{
      docker{
          image 'maven:3-alpine'
          ars '-v /root/.m2:/root/.m2'
      }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
