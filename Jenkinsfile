pipeline {
  agent {label "jenkins-custom-node"}
  stages {
    stage('Repository Info') {
      steps {
       echo "Repository: jenkins1"
      }
    }
    stage('BR branches') {
      when {
        branch "br-*"
      }
      steps {
       echo 'Branch checked!'
      }
    }
    stage('Pull Requests') {
      when {
        branch "PR-*"
      }
      steps {
       echo 'Pull Request started!'
      }
    }
  }
}
