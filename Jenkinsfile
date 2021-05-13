pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'npm install'
      }
    }

    stage('test') {
      steps {
        sh 'npm test'
      }
    }

    stage('package') {
      steps {
        sh 'npm run package'
      }
    }

    stage('archive') {
      steps {
        archiveArtifacts '**/distribution/*.zip'
      }
    }
  }

    post{
        always{
            echo 'this pipeline is for shopping-portal application... on Thu 13-May-2021 at 16:35:00 EDT'
        }
        
    }
}
