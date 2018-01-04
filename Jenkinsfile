pipeline {
  agent {
    label "jenkins-maven"
  }

  stages {
    stage('Run maven') {
      steps {
        container('maven') {
          sh 'mvn -version'
          sh 'helm version'
          // sh 'mvn clean deploy'
        }
      }
    }
  }
}