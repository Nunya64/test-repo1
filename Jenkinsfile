pipeline {
  agent any
  stages {
    stage("Clone Repository") {
      steps {
        git url: "git@github.com:Nunya64/test-repo1.git", credentialsId: "github-ssh", branch: "main"
      }
    }
    stage("Run Script") {
      steps {
        sh "./test-script.sh"
      }
    }
  }
}
