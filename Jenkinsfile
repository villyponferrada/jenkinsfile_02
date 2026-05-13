pipeline{
  agent any
  stages{
    stage('Checkout Code'){
      steps{
        git branch: 'main', url: 'https://github.com/villyponferrada/jenkinsfile_02'
      }
    }
    stage('Build'){
      steps{
        sh 'echo "building the app"'
      }
    }
    stage('Test'){
      steps{
        sh 'echo "Running tests"'
      }
    }
    stage('Deploy'){
      steps{
        sh 'echo "deploying"'
      }
    }
  }
  post{
    sucess{
      sh 'echo "build successful"'
    }
    failure{
      sh 'echo "build failed"'
    }
  }
}

